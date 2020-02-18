---
title: Elecciones Perú 2020
havechart: true
---

<p>
    Cerca de 25 millones de peruanos elegirán a los 130 congresistas que ocuparán el recinto por un periodo de 18 meses, es decir, hasta las elecciones nacionales de 2021, que redefinirán nuevamente su composición
</p>
<div style=" max-width: 350px;">
<canvas id="myChart" width="100" height="100"></canvas>

</div>

<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'pie',
    data: {
        labels: ['Hab Inscritos', 'Población'],
        datasets: [{
            data: [24799384,32495500 ],
            backgroundColor: [
                'yellow',
                'blue',
                
            ],
          
        }],
       
    },
     options: {
				responsive: true
			}

});
</script>
