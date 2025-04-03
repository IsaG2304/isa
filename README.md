<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clasificador MNIST</title>
    <script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
</head>
<body>
    <h1>Prueba el modelo MNIST en la web</h1>
    <input type="file" id="imageInput">
    <script>
        async function cargarModelo() {
            const modelo = await tf.loadLayersModel('model.json');
            console.log("Modelo cargado correctamente");
        }
        cargarModelo();
    </script>
</body>
</html>
