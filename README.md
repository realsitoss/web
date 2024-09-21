
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>21 de Septiembre - Día de las Flores</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <div class="container">
    <!-- Primera sección con el poema -->
    <div class="section" id="section1">
      <h1>Amor</h1>
      <p class="poema">En este día tan especial, <br> quiero recordarte lo mucho que te amo. <br> Eres mi flor más hermosa, <br> y mi vida florece cuando estás cerca.</p>
      <button class="button" id="nextBtn">Siguiente</button>
    </div>

    <!-- Segunda sección con las flores y los poemas largos -->
    <div class="section" id="section2" style="display: none;">
      <img src="file:///C:/Users/cuent/Pictures/flores.jfif" alt="Flores amarillas" class="flores-img">
      <div class="poemas-largos">
        <p class="poema-largo">A tu lado he encontrado la paz, <br> una calma que nunca imaginé. <br> Tus sonrisas son como las flores, <br> llenan mi vida de color.</p>
        <p class="poema-largo">El amor florece en tu presencia, <br> como el sol que da vida a la tierra. <br> Gracias por ser mi flor eterna, <br> mi alegría en cada primavera.</p>
      </div>
      <button class="button" id="touchMeBtn">Tócame</button>
    </div>

    <!-- Tercera sección con el video -->
    <div class="section" id="section3" style="display: none;">
      <h2>Y ahora una canción para ti</h2>
      <iframe width="560" height="315" src="https://youtu.be/WiinVuzh4DA?si=gkcr3LNPXGsrK0Pl" title="pa ti" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </div>

  <script>
    const nextBtn = document.getElementById('nextBtn');
    const touchMeBtn = document.getElementById('touchMeBtn');
    const section1 = document.getElementById('section1');
    const section2 = document.getElementById('section2');
    const section3 = document.getElementById('section3');

    // Mostrar la segunda sección al hacer clic en "Siguiente"
    nextBtn.addEventListener('click', function() {
      section1.style.display = 'none';
      section2.style.display = 'block';
    });

    // Mostrar la tercera sección (el video) al hacer clic en "Tócame"
    touchMeBtn.addEventListener('click', function() {
      section2.style.display = 'none';
      section3.style.display = 'block';
    });
  </script>

</body>
</html>
