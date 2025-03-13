<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Gastos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
            display: flex;
            justify-content: space-around;
        }
        .container {
            width: 40%;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 10px;
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
        }
        input, button {
            margin-top: 10px;
            display: block;
            width: 100%;
        }
        .barra {
            height: 20px;
            margin-top: 10px;
            border-radius: 5px;
        }
        .azul { background-color: blue; width: 0%; }
        .rosado { background-color: pink; width: 0%; }
    </style>
</head>
<body>
    <div class="container">
        <h2>Gastos Azul</h2>
        <p>Total Azul: <span id="totalAzul">0</span> ₪</p>
        <input type="number" id="montoAzul" placeholder="Ingrese un monto">
        <input type="text" id="descripcionAzul" placeholder="Descripción del gasto">
        <button onclick="agregarGasto('azul')">Agregar a Azul</button>
        <div class="barra azul" id="barraAzul"></div>
        <h3>Historial de Gastos</h3>
        <ul id="historialAzul"></ul>
    </div>
    
    <div class="container">
        <h2>Gastos Rosado</h2>
        <p>Total Rosado: <span id="totalRosado">0</span> ₪</p>
        <input type="number" id="montoRosado" placeholder="Ingrese un monto">
        <input type="text" id="descripcionRosado" placeholder="Descripción del gasto">
        <button onclick="agregarGasto('rosado')">Agregar a Rosado</button>
        <div class="barra rosado" id="barraRosado"></div>
        <h3>Historial de Gastos</h3>
        <ul id="historialRosado"></ul>
    </div>
    
    <script src="script.js"></script>
</body>
</html>
