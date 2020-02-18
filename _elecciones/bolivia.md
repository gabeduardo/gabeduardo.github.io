---
title: Elección presidencial y legislativa Bolivia 2020
havechart: true
---

La celebración de nuevos comicios presidenciales y legislativos en Bolivia aún no tiene fecha, pero la autoproclamada presidenta interina, Jeanine áñez, ya promulgó la Ley de Régimen Excepcional y Transitorio para la Realización de Elecciones Generales, que anula los resultados de los comicios del 20 de octubre.

Se estima que la convocatoria oficial la realice el Tribunal Supremo Electoral (TSE) el próximo 2 de enero. Por ahora, Áñez ha advertido que Morales no podrá participar en las elecciones, debido a que está —dijo— "inhabilitado" para hacerlo.

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
            data: [71315364,116333713 ],
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
