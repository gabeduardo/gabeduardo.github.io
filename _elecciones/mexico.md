---
title: Elecciones federativas Mexico 2020
havechart: true
meta: Las elecciones de México de 2020 son el conjunto de elecciones coordinadas por el Instituto Nacional Electoral (INE) y los Organismos Públicos Locales de Elecciones (OPLE) para renovar diversos cargos en dos entidades federativas de ese país en el año 2020 (...)
---

![bandera-mexico](/images/mexico.jpg)

<p>
    En México, habrá elecciones en dos de las 32 entidades federativas el 7 de junio de 2020.

De acuerdo al Instituto Nacional Electoral (INE), en Hidalgo se elegirán los titulares de 84 ayuntamientos; mientras, en el estado de Coahuila se renovará el congreso local, de 25 diputados.

</p>

[Fuente de datos utilizada ](https://aginformacion.tv/mexico-sobre-el-padron-electoral-y-los-datos-biometricos/)

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
         pointHoverBackgroundColor: 'beige'
          
        }],
       
    },
    options: {
        legend: {
            display: true,
            labels: {
                fontColor: 'black',
               
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
                    return 'white';
                }
            }
        }
    }
    

});
</script>
