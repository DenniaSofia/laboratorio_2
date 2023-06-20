# laboratorio_2
Esta es una web que consiste en elaborar una lista de tareas. En ella puedes agregar la cantidad de tareas que prefieras e 
ir eliminando aquellas que ya hayas realizado. Fue elaborada como práctica en la clase de Diseño Web para los estudiantesde tercer 
año de Diseño Gráfico y Multimedia. Se utilizó el programa de Visual Studio Code, insertando los códigos correspondientes al html, 
css y java script facilitados por el docente. A continuación, se detalla la estructura que está detrás de este segundo ejercicio:

ARCHIVO HTML
Este archivo es el texto de la página web, que está «marcado» con estos códigos para dar instrucciones al navegador web 
obre cómo mostrar el texto.

<!DOCTYPE html>
<html>
<head>
<title>Lista de tareas</title>
<link rel="stylesheet" type="text/css" href="estilos.css">
</head>
<body>
<h1>HAZ TU LISTA DE TAREAS</h1>
<div id="task-container">
<input type="text" id="task-input" placeholder="Agregar nueva tarea">
<button id="add-task-btn">Agregar</button>
</div>
<ul id="task-list">
<!-- Aquí se agregarán las tareas dinámicamente -->
</ul>
<script src="app.js"></script>
</body>
</html>

ARCHIVO CSS
