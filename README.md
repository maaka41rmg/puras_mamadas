# puras_mamadas
lo mejor del mundo
 <!DOCTYPE html>
<html>
<head>
	<title>Generador de ideas</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<style>
		body {
			font-family: Arial, sans-serif;
			text-align: center;
		}
		h1 {
			margin-top: 50px;
		}
		button {
			margin-top: 30px;
			padding: 10px 20px;
			background-color: #4CAF50;
			color: white;
			border: none;
			border-radius: 5px;
			cursor: pointer;
		}
	</style>
</head>
<body>
	<h1>Generador de ideas</h1>
	<p>Haz clic en el botón para generar una idea:</p>
	<button onclick="generarIdea()">Generar idea</button>
	<p id="frase"></p>

	<script>
		// Arreglos de lugares, objetivos y emociones
		var lugares = ["en la playa", "en la montaña", "en una ciudad", "en un parque", "en un restaurante", "en un museo", "en un concierto", "en una fiesta", "en el cine", "en casa"];
		var objetos = ["una bicicleta", "un libro", "una cámara", "un teléfono", "una guitarra", "un cepillo de dientes", "un reloj", "un par de zapatos", "un sombrero", "un paraguas"];
		var emociones = ["feliz", "emocionado/a", "nervioso/a", "triste", "enojado/a", "asombrado/a", "relajado/a", "abrumado/a", "sorprendido/a", "preocupado/a"];

		// Función para generar la idea aleatoria
		function generarIdea() {
			var lugar = lugares[Math.floor(Math.random() * lugares.length)];
			var objeto = objetos[Math.floor(Math.random() * objetos.length)];
			var emocion = emociones[Math.floor(Math.random() * emociones.length)];
			document.getElementById("frase").innerHTML = "Quiero estar " + lugar + ", con " + objeto + " y sentirme " + emocion + ".";
		}
	</script>
</body>
</html>
