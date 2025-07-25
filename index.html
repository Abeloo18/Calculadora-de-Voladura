<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Calculadora de Distancia Segura - Voladura Minera</title>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    body { font-family: Arial, sans-serif; padding: 20px; }
    input, label, button { display: block; margin-top: 10px; }
    canvas { margin-top: 30px; max-width: 600px; }
  </style>
</head>
<body>
  <h2>Calculadora de Distancia Segura y PPV</h2>

  <label for="w">Carga explosiva (W) en kg:</label>
  <input type="number" id="w" value="50">

  <label for="k">Constante del terreno (K):</label>
  <input type="number" id="k" value="1000">

  <label for="n">Exponente (n):</label>
  <input type="number" id="n" value="1.6">

  <label for="ppv_lim">PPV permitida (mm/s):</label>
  <input type="number" id="ppv_lim" value="10">

  <button onclick="calcular()">Calcular distancia segura</button>

  <p id="resultado"></p>

  <canvas id="grafico"></canvas>

  <script>
    function calcularPPV(k, w, r, n) {
      return k * Math.pow(w / Math.pow(r, n), 1);
    }

    function calcular() {
      const w = parseFloat(document.getElementById('w').value);
      const k = parseFloat(document.getElementById('k').value);
      const n = parseFloat(document.getElementById('n').value);
      const ppv_lim = parseFloat(document.getElementById('ppv_lim').value);

      let r_segura = Math.pow((k * w) / ppv_lim, 1 / n);

      document.getElementById('resultado').textContent =
        `Distancia mínima segura: ${r_segura.toFixed(2)} metros`;

      // Gráfico
      let distancias = [];
      let ppvs = [];

      for (let r = 1; r <= r_segura * 1.5; r += 1) {
        distancias.push(r);
        ppvs.push(calcularPPV(k, w, r, n));
      }

      const ctx = document.getElementById('grafico').getContext('2d');
      new Chart(ctx, {
        type: 'line',
        data: {
          labels: distancias,
          datasets: [{
            label: 'PPV (mm/s)',
            data: ppvs,
            borderColor: 'blue',
            fill: false
          }]
        },
        options: {
          responsive: true,
          plugins: {
            title: {
              display: true,
              text: 'PPV vs Distancia'
            }
          },
          scales: {
            x: {
              title: { display: true, text: 'Distancia (m)' }
            },
            y: {
              title: { display: true, text: 'PPV (mm/s)' }
            }
          }
        }
      });
    }
  </script>
</body>
</html>

