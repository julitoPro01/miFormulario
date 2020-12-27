<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        label{
            display: block; margin: 5px;
        }
    </style>
    <script>
        window.onload = function (){
            var formulario = document.forms;
            for(var i=0;i<formulario.length;i++){
                for(var j=0;j<formulario[i].elements.length;j++){
                if(formulario[i].elements[j].type == 'text'){
                    formulario[i].elements[j].addEventListener('click',cambiarColor);
                }
            }
        }
           }
        function cambiarColor(){
            
            this.style.backgroundColor = 'yellow';
        }
    </script>
</head>
<body>
    <div id="cabecera"><h2>curso aprendoaprogramar.com</h2><h3>ejemplos javascript</h3></div>
    <form action="#" name="formularioContacto" method="get" >
        <h2>formulario de contacto</h2>
        <label for="">Nombre <input type="text" id="nombreFormContacto" name="nombre" maxlength="4"></label>
        <label for="">Apellidos <input type="text" id="apellidosFormContacto" name="apellidos"></label>
        <label for=""><input type="submit" id="botonEnvio1" value="Enviar"></label>
    </form>
    <form action="#" name="formulairoReclamacion" method="get">
        <h2>formulario de reclamacion</h2>
        <label for="">Motivo reclamacion: <input type="text" id="motivoFormReclama" name="motivo"></label>
        <label for="">Fecha de hecho: <input type="text" id="fechaFormReclama" name="fecha"></label>
        <label for=""><input type="submit" id="botonEnvio2" value="Enviar"></label>
    </form>
</body>
</html>
