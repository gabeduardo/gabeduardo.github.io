---
title: Plebiscito nacional de Chile de 2020
havechart: true
meta: Este país suramericano también acudirá a las urnas en octubre. Por primera vez elegirán, mediante el voto popular(...)
---

![bandera-chile](/images/chile.jpg)

<p>
Este país suramericano también acudirá a las urnas en octubre. Por primera vez elegirán, mediante el voto popular, a los gobernadores regionales, 16 en total, que estarán a cargo de igual número de regiones chilenas; hasta ahora ese puesto era de un intendente, quien era nombrado por el Presidente de la República, pero cambió a partir de la publicación de la Ley 21.073 de 2018.

La primera vuelta será el 25 de octubre y, en caso de que ningún candidato obtenga el 40 % de los votos válidamente emitidos, habrá un balotaje el 22 de noviembre

</p>
[Fuente de datos utilizada ](https://es.wikipedia.org/wiki/Plebiscito_nacional_de_Chile_de_2020)

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
            data: [14695245,19107216 ],
            backgroundColor: [
                'yellow',
                'blue',
                
            ],
            pointHoverRadius: 5,
         pointHoverBackgroundColor: 'red'
          
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
