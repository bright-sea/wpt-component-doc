                    "compactForm":1,
                    "rowHeaderWidth":200,
                    "cellWidth":100,
                    "cellHeight":23,
                    "theme":"wpt-default"
                },  
                "chart":{
                    "width":500,
                    "height":300,
                    "high":{
                        "theme":"default",  //default, grid, gray, skies, drak-blue, drak-green
                        chart:{
                            type:'column',  //column, bar, line, spline, area, areaspline, pie
                            options3d: {
                                enabled: false,
                                alpha: 15,
                                beta: 15,
                                depth: 50,
                                viewDistance: 25
                            }
                        },
                            credits: {
                                enabled:false
                            },
                            exporting: {
                                enabled:true
                            },
                            navigation:{
                                buttonOptions:{
                                    align: 'right',   // left, center, right
                                    verticalAlign: 'top' // top, middle, bottom
                                }
                            },
                            legend: {
                                enabled: true,
                                floating: false,
                                layout: 'vertical',  //horizontal, vertical
                                align: 'right',      // left, center, right
                                verticalAlign: 'middle', // top, middle, bottom
                                reversed: false
                            },
                            tooltip:{
                                enabled: true,
                                shadow: true
                            },
                            plotOptions: {
                                series:{
                                    stacking: null //null, 'normal', "percent"
                                }
                            },
                            xAxis: {
                                labels:{
                                    enabled: true,