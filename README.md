# footerAKU
Footer de Akutangulo.com para mostrar en las webs


<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, maximum-scale=1">
<link rel="icon" href="https://akutangulo.com/images/logo-akutangulo-diseño-web-seo.svg">
<title>Akutangulo diseño de páginas web, posicionamiento SEO y fotografía pánorámica para empresas en Valladolid</title>

<!---------------------------------->
<style>
@font-face {
font-family: 'bauhouse_akutangulo';
src: url('bauhouse_akutangulo.eot'); /* archivo EOT para IE */ 
src: url('bauhouse_akutangulo.eot?#iefix') format('embedded-opentype'),
url('bauhouse_akutangulo.ttf') format('truetype'); /* archivo TTF para navegadores CSS3 */
}

body {
background:#000;
overflow-x: hidden;
}

.akutangulo-diseño-web-seo {
  font-family: 'bauhouse_akutangulo';
  color: #9400D3;
  animation:glow 10s ease-in-out infinite;
}

.aku-container {
  position: relative; 
  top: 0; /* Se coloca en la parte superior */
  width: 100%; /* Ocupa todo el ancho de la pantalla */
}

.aku {
  font-family: 'bauhouse_akutangulo';
  color: #9400D3;
  animation:wobble 5s ease-in-out infinite;
  transform-origin:center center;
  transform-style:preserve-3d;
  display: flex;
  justify-content: center; /* Centra horizontalmente */
  align-items: center; /* Centra verticalmente */
  height: 150px; /* Altura fija del contenedor */

  
}
span.aku {
  text-align:center;
  z-index: 100;
  display:block;
  padding:4px;
  line-height:1.5;
  text-transform:none;
  position:absolute;
  animation:glow 10s ease-in-out infinite;
  font-size: calc(4rem + 2.3vw); 

}

@keyframes glow {
0%,100%{ text-shadow:0 0 30px DeepPink; }
25%{ text-shadow:0 0 30px Lime; }
50%{ text-shadow:0 0 30px Magenta; }
75%{ text-shadow:0 0 30px MediumSlateBlue; }
}

@keyframes wobble {
  0%, 100% { transform: rotate3d(1, 1, 0, 40deg); } /* Giro hacia los lados */
  25% { transform: rotate3d(-1, 1, 0, 25deg); } /* Giro hacia abajo con menos ángulo */
  50% { transform: rotate3d(-1, -1, 0, 40deg); } /* Giro hacia los lados */
  75% { transform: rotate3d(1, -1, 0, 25deg); } /* Giro hacia arriba con menos ángulo */
}
span:nth-child(2){ transform:translateZ(5px); }
span:nth-child(3){ transform:translateZ(10px); }
span:nth-child(4){ transform:translateZ(15px); }
span:nth-child(5){ transform:translateZ(20px); }
span:nth-child(6){ transform:translateZ(25px); }
span:nth-child(7){ transform:translateZ(30px); }
span:nth-child(8){ transform:translateZ(35px); }

.footer {
    padding: 20px;
    text-align: center;
    }	
    .footer-logo {
    margin:15px auto;
    width: 76px;
    }
    .copyright {
    color:#cccccc;
    font-size: 1rem;
    }
    .copyright a {
    text-decoration: none; 
    transition:all 0.3s ease-in-out;
    -moz-transition:all 0.3s ease-in-out;
    -webkit-transition:all 0.3s ease-in-out;
    }
    .copyright a:hover {
    font-size: larger;
    }

    /* Estilo base para el trazado del logo Akutangulo en svg*/
.animacion-logo-svg {
    fill: none;
    stroke: #9300D3; /* Color del trazado */
    stroke-width: 5; /* Ancho del trazado */
    stroke-dasharray: 3000; /* Longitud total del trazado */
    stroke-dashoffset: 3000; /* Desplazamiento inicial, oculta el trazado */
    animation: draw 5s ease-in-out forwards, fillLogo 2s ease-in-out forwards 3s, glow 10s ease-in-out infinite;
    }
    
    /* Animación para dibujar el trazado del logo Akutangulo */
    @keyframes draw {
    0% {
    stroke-dashoffset: 3000; /* Comienza con el trazado completamente oculto */
    }
    100% {
    stroke-dashoffset: 0; /* Desplazamiento final, muestra todo el trazado */
    }
    }
    
    /* Animación para rellenar el logo con color */
    @keyframes fillLogo {
    0% {
    fill: transparent; /* Comienza con el relleno transparente */
    }
    50% {
    fill: #fbf8fb; /* Termina con el color de relleno */
    }
    100% {
    fill: #9300D3; /* Termina con el color de relleno */
    }
    }
</style>
</head>
<body>
 <header>
  <div class="aku-container">
 <figure class="aku">
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
		<span class="aku">Akutangulo</span>
    <span class="aku">Akutangulo</span>
 </figure>
</div>

 </header>

<nav>

</nav>

<div style="height: 800px;"><p class="akutangulo-diseño-web-seo" style="color: #fff; font-size: 2rem; padding: 2rem;">Akutangulo, diseño y creación de páginas web, posicionamiento SEO y fotógrafo oficial de google maps street view trusted en valladolid</p></div>


<footer class="footer">
<div class="container">
      <div class="footer-logo">
        <a href="https://akutangulo.com">
          <svg xmlns="http://www.w3.org/2000/svg" version="1.0" width="65.000000pt" height="65.000000pt" viewBox="0 0 58.000000 67.000000" preserveAspectRatio="xMidYMid meet">
           <metadata>Logo de Akutangulo, diseño y creación de páginas web, posicionamiento SEO y fotógrafo oficial de google maps street view trusted en valladolid. Oscar Navarro. </metadata>
           <g transform="translate(0.000000,65.000000) scale(0.100000,-0.100000)" fill="#9300D3" stroke="none">
           <path class="animacion-logo-svg" d="M175 551 c-112 -52 -169 -207 -120 -329 19 -45 86 -112 172 -169 51 -35 52 -35 77 -16 24 17 25 22 26 125 l0 106 -38 -5 c-51 -7 -77 21 -68 72 8 42 41 60 80 45 40 -15 46 -40 46 -182 l0 -133 90 9 90 10 0 156 c0 147 -1 159 -25 207 -26 51 -72 91 -128 112 -46 18 -157 13 -202 -8z"/>
           </g>
           </svg>          
        </a>
      </div>

    <div class="copyright">
      <p>Web diseñada con amor ❤️ por <a href="https://akutangulo.com" rel="noopener" target="_blank" title="Akutangulo - Páginas web y posicionamiento S.E.O." aria-label="Akutangulo - Páginas web y posicionamiento SEO" class="akutangulo-diseño-web-seo">Akutangulo.com</a></p>

      <p>Copyright © <span id="copyright-year"></span> by <a href="https://akutangulo.com" rel="noopener" target="_blank" title="Akutangulo - Páginas web y posicionamiento S.E.O." aria-label="Akutangulo - Páginas web y posicionamiento SEO" class="akutangulo-diseño-web-seo">Akutangulo</a></p>   
    </div>

</div>
</footer>

<script>
//Se asigna directamente el año actual al contenido del elemento span con id="copyright-year" utilizando textContent. La función new Date().getFullYear() se utiliza para obtener el año actual de forma dinámica
document.getElementById("copyright-year").textContent = new Date().getFullYear();
</script>

</body>
</html>
