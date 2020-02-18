---
title: Elecciones federativas Mexico 2020
havechart: true
---

En México, habrá elecciones en dos de las 32 entidades federativas el 7 de junio de 2020.

De acuerdo al Instituto Nacional Electoral (INE), en Hidalgo se elegirán los titulares de 84 ayuntamientos; mientras, en el estado de Coahuila se renovará el congreso local, de 25 diputados.

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
            data: [89903166,126577691 ],
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
