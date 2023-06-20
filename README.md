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
La hoja de estilo CSS se utiliza para dar un formato adecuado al HTML. De este modo, se definieron atributos como el diseño, el color y la forma de los elementos individuales de HTML.

body {
    font-family: Arial, sans-serif;
    background-color: #474646;
    margin: 0;
    padding: 20px;
    }
    h1 {
    text-align: center;
    color: #c0d3ff;
    }
    #task-container {
    display: flex;
    margin-bottom: 20px;
    }
    #task-input {
    flex-grow: 1;
    padding: 10px;
    font-size: 16px;
    }
    #add-task-btn {
    padding: 10px 20px;
    background-color: #0084ff;
    border: none;
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    }
    #task-list {
    list-style-type: none;
    padding: 0;
    }
    .task-item {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #fff;
    padding: 10px;
    margin-bottom: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }
    .task-item span {
    flex-grow: 1;
    margin-right: 10px;
    }
    .delete-btn {
    background-color: #ff0000;
    border: none;
    color: #fff;
    padding: 5px 10px;
    font-size: 14px;
    border-radius: 3px;
    cursor: pointer;
    }
    .fade-in {
    animation: fade-in 0.5s;
    }
    @keyframesfade-in {
    from {
    opacity: 0;
    transform: translateY(-10px);
    }
    to {
    opacity: 1;
    transform: translateY(0);
    }
    }

    ARCHIVO JAVA SCRIPT
    
