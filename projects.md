---
title: Projets
layout: home
description: "3 anneaux pour les embarquer tous"
---
<div class="row">
    <div id="container" style="height: 700px"></div>
    <script type="text/javascript">
    var dom = document.getElementById('container');
    var myChart = echarts.init(dom, null, {
      renderer: 'canvas',
      useDirtyRect: false
    });
    var app = {};
    var option;

    myChart.showLoading();
    $.getJSON('/assets/projects.json', function (graph) {
    myChart.hideLoading();
    graph.nodes.forEach(function (node) {
        node.label = {
        show: node.symbolSize > 30
        };
    });
    option = {
        title: {
        text: 'Interactions des projets au sein du tiers-lieu',
        top: 'auto',
        left: 'center'
        },
        tooltip: {},
        toolbox: {
            show: true,
            feature: {
                restore: {},
                saveAsImage: {}
            }
        },
        legend: [
        {
            // selectedMode: 'single',
            data: graph.categories.map(function (a) {
            return a.name;
            })
        }
        ],
        animationDuration: 1500,
        animationEasingUpdate: 'quinticInOut',
        series: [
        {
            name: 'Tiers lieu La Vauzelle',
            type: 'graph',
            legendHoverLink: false,
            layout: 'none',
            data: graph.nodes,
            links: graph.links,
            categories: graph.categories,
            roam: true,
            label: {
            position: 'right',
            formatter: '{b}'
            },
            lineStyle: {
            color: 'source',
            curveness: 0.3
            },
            emphasis: {
            focus: 'adjacency',
            lineStyle: {
                width: 10
            }
            }
        }
        ]
    };
    myChart.setOption(option);
    });

        if (option && typeof option === 'object') {
        myChart.setOption(option);
        }

        window.addEventListener('resize', myChart.resize);
    </script>
  </div>