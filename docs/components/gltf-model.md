<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AR Arduino</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
</head>
<body style="margin: 0; overflow: hidden;">
    <a-scene embedded arjs="sourceType: webcam; debugUIEnabled: false;">
        <!-- Définir le marqueur -->
        <a-marker type="pattern" url="path/to/your-marker.patt">
            <!-- Ajouter le modèle 3D de la carte Arduino -->
            <a-entity
                gltf-model="path/to/arduino-model.glb"
                scale="0.01 0.01 0.01"
                position="0 0 0"
                rotation="0 0 0">
            </a-entity>
        </a-marker>
        <!-- Caméra AR -->
        <a-entity camera></a-entity>
    </a-scene>
</body>
</html>
