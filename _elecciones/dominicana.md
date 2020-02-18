---
title: Elecciones República Dominicana 2020
havechart: true
---

Los comicios en República Dominicana serán generales y están convocados para el 17 de mayo. Quien resulte electo será el sucesor de Danilo Medina, que gobierna el país desde 2012.

En las elecciones primarias partidarias de octubre pasado se eligieron a dos candidatos; sin embargo, el número de aspirantes es más amplio.

<div style=" max-width: 350px;">
<canvas id="myChart" width="100" height="100"></canvas>

</div>

<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
        labels: ['Votantes disp', 'Población total'],
        datasets: [{
            data: [7340868,11088647 ],
            backgroundColor: [
                'yellow',
                'blue',
                
            ],
            pointHoverRadius: 5,
         pointHoverBackgroundColor: 'black'
          
        }],
       
    },
    options: {
        legend: {
            display: true,
            labels: {
                fontColor: 'black',
                padding	: 86
            }
        },


         tooltips: {
            callbacks: {
                labelColor: function(tooltipItem, chart) {
                    return {
                        borderColor: 'black',
                        backgroundColor: 'rgb(255, 0, 0)'
                    };
                },
                labelTextColor: function(tooltipItem, chart) {
                    return 'black';
                }
            }
        }
    }
    

});
</script>
