---
title: Elecciones Perú 2020
havechart: true
meta: En el Perú, constituyó un proceso electoral especial que se llevó a cabo el domingo 26 de enero de 2020, como consecuencia de la disolución del Congreso de la República por parte del presidente Martín Vizcarra el 30 de septiembre de 2019 en aplicación del artículo 134 de la Constitución Política del Perú (...)
---

![bandera-peru](/images/peru.jpg)

<p>
    Cerca de 25 millones de peruanos elegirán a los 130 congresistas que ocuparán el recinto por un periodo de 18 meses, es decir, hasta las elecciones nacionales de 2021, que redefinirán nuevamente su composición

</p>

[Fuente de datos utilizada ](https://es.wikipedia.org/wiki/Elecciones_parlamentarias_extraordinarias_de_Per%C3%BA_de_2020)

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
            data: [24799384,32495500 ],
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
