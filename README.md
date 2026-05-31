# CV_JS
Mi CV creado en HTML  y CSSS


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Curriculum</title>
</head>
<body>
 <!-- Contenedor principal del CV -->
    <div class="cv-container">

        <!-- LADO IZQUIERDO  (barra lateral) -->
        <div class="sidebar">

             <!-- Sección de foto de perfil -->
            <div class="profile">
            <!-- Imagen del perfil (vacía porque no hay ruta en src) -->
                <img src="" alt="Foto de perfil">
            </div>

            <!-- CONTACTO -->
            <div class="section">
                <h3>DATOS DE CONTACTO</h3>
                <!-- Teléfono -->
                <p>📞 Contacto: +52 33 18674448</p><br>
                <!-- Correo electrónico -->
                <p>📧 Correo: jspgonzalez1603@gmail.com</p><br>
            </div>

            <!-- COMPETENCIAS -->
            <div class="section">
                <h3>COMPETENCIAS</h3>
                <!-- Lista de habilidades -->
                <ul>
                    <li>Adaptabilidad y respeto en entornos diversos.</li>
                    <li>Habilidad para trabajar en equipo y alcanzar objetivos comunes. </li>
                    <li>Comunicación asertiva y clara en entornos profesionales. </li>
                    <li>Competencias en TIC aplicadas al entorno laboral.</li>
                    <li>Compromiso con el aprendizaje continuo y la mejora constante. </li>
                </ul>
            </div>

            <!-- IDIOMAS -->
            <div class="section">
                <h3>IDIOMAS</h3>

                <p>Español</p>
                <p>Inglés básico</p>
            </div>

        </div>

        <!-- LADO DERECHO (contenido principal del CV) -->
        <div class="main-content">

            <!-- Encabezado con nombre y profesión -->
            <div class="header">
                <h1>JOEL SALVADOR</h1>
                <h1>GONZALEZ PAOLOMERA</h1>
                <h2>ING. SISTEMAS</h2>
            </div>

            <!-- OBJETIVO -->
            <div class="content-section">

                <h3>OBJETIVO PROFESIONAL</h3>

                <div class="item">
                    <p>Desarrollarme profesionalmente en un entorno que me permita
                        aplicar los conocimientos adquiridos en mi carrera,
                        al mismo tiempo que continúo aprendiento y aportando
                        al logro de los objetivos de la organización. </p>
                </div>

             <!-- EXPERIENCIA -->
                <h3>EXPERIENCIA LABORAL</h3>

                <div class="item">
                    <h4>2021 - 2026</h4>
                    <!-- Nombre de la empresa -->
                    <p><strong>Empresa de Prefabricados Carrillo S.A de C.V</strong></p>
                    <p>Principales funciones:</p>
                     <!-- Lista de funciones -->
                    <P>1. Operador de maquina automatizada <br>
                        2. Mantenimiento general
                    </P>

                </div>
            </div>

            <!-- EDUCACIÓN -->
            <div class="content-section">
                <h3>EDUCACIÓN</h3>

                <div class="item">
                    <h4>2023 - 2026</h4>
                    <p><strong>UTEG: Universidad Tecnológica de Guadalajara</strong></p>
                    <p>Licenciatura en Ing.Sistemas</p>
                </div>
            </div>

             <!-- HABILIDADES -->

            <div class="content-section">
                <h3>HABILIDADES TÉCNICAS</h3>

                <div class="item">
                    <p> 1. Conocimiento en el manejo de paqueteria OFFICE. <br>
                        2. Conocimiento en redes (Cableado estructurado, 
                        configuracion de Routers, Switch, instalacion de camaras, etc.) <br>
                        3. Programacion basica en lenguaje como:
                         
                        <!-- Lista de lenguajes -->
                        <ul>
                                <li>JavaScript</li>
                                <li>C#</li>
                                <li>MySQL</li>
                                <li>SQL server</li>
                        <p><strong>Y otros como:</strong></p>
                                <li>HTML</li>
                                <li>CSS</li>
                                <li>PHP</li>
                        </ul>
                    </p>
                </div>
            </div>

        </div>

    </div>

</body>
</html>


CSS 

*{
    margin: 0; /* elimina márgenes por defecto */
    padding: 0; /* elimina rellenos por defecto */
    box-sizing: border-box; /* incluye padding y border dentro del tamaño del elemento */
    font-family: Arial, Helvetica, sans-serif; /* fuente general del CV */
}

body{
    background: #d9d9d9; /* color gris claro de fondo */
    display: flex; /* activa flexbox */
    justify-content: center; /* centra horizontalmente el CV */
    padding: 30px; /* espacio alrededor del CV */
}

.cv-container{
    width: 900px; /* ancho fijo del CV */
    background: white; /* fondo blanco tipo hoja */
    display: flex; /* coloca sidebar y contenido en fila */
    box-shadow: 0 0 20px rgba(0,0,0,0.2); /* sombra suave alrededor */
}

.sidebar{
    width: 35%; /* ocupa 35% del ancho total */
    background: #0d2b52; /* azul oscuro profesional */
    color: white; /* texto blanco */
    padding: 30px; /* espacio interno */
}

.profile{
    display: flex; /* usa flexbox */
    justify-content: center; /* centra la imagen horizontalmente */
    margin-bottom: 30px; /* separación inferior */
}


.profile img{
    width: 140px; /* ancho de la imagen */
    height: 140px; /* alto de la imagen */
    border-radius: 50%; /* convierte la imagen en círculo */
    border: 5px solid white; /* borde blanco alrededor */
    object-fit: cover; /* recorta la imagen sin deformarla */
}


.section{
    margin-bottom: 30px; /* separación entre secciones */
}

/* títulos del sidebar */
.section h3{
    font-size: 18px; /* tamaño del título */
    margin-bottom: 15px; /* separación inferior */
    border-bottom: 2px solid white; /* línea decorativa debajo */
    padding-bottom: 5px; /* espacio entre texto y línea */
}

/* texto y elementos de lista */
.section p,
.section li{
    font-size: 14px; /* tamaño de texto pequeño */
    line-height: 1.6; /* espacio entre líneas */
}

/* listas del sidebar */
.section ul{
    padding-left: 20px; /* sangría para viñetas */
}

/* LADO DERECHO  */
.main-content{
    width: 65%; /* ocupa el resto del espacio */
    padding: 40px; /* espacio interno */
}

.header{
    margin-bottom: 40px; /* separación inferior */
}

/* nombre principal */
.header h1{
    font-size: 30px; /* tamaño grande */
    color: #0d2b52; /* mismo azul del sidebar */
    line-height: 1; /* reduce espacio entre líneas */
}

/* profesión */
.header h2{
    font-size: 24px; /* tamaño medio */
    color: gray; /* color neutro */
    margin-top: 10px; /* separación superior */
    letter-spacing: 3px; /* separa letras para estilo elegante */
}

.content-section{
    margin-bottom: 40px; /* separación entre bloques */
}

/* títulos de sección */
.content-section h3{
    color: #0d2b52; /* azul principal */
    font-size: 22px; /* tamaño del título */
    margin-bottom: 20px; /* separación inferior */
    border-bottom: 2px solid #0d2b52; /* línea decorativa */
    padding-bottom: 5px; /* espacio con la línea */
}

.item{
    margin-bottom: 25px; /* separación entre elementos */
}

/* fechas o subtítulos */
.item h4{
    color: #0d2b52; /* azul destacado */
    margin-bottom: 5px; /* separación inferior */
}

/* párrafos dentro de items */
.item p{
    margin-bottom: 5px; /* separación entre párrafos */
    color: #444; /* gris oscuro para lectura cómoda */
    text-align: justify; /* texto alineado tipo documento */
    line-height: 1.6; /* mejor lectura */
}

/* listas dentro de items */
.item ul{
    padding-left: 30px; /* sangría de lista */
    line-height: 1.6; /* espacio entre elementos */
}
