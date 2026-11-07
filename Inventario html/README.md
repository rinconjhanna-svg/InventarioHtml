# Proyecto de html5, css3, Bootstrap5
Este proyecto es una plantilla de gestion de
 inventarios para un administrador de sistema

 - Contiene:
 - Inicio de sesion
 - Dashboar
 - gestion de usuarios
 - gestion de categoria
 - gestion de subcategoria 
 - gestion de productos
 **Todas las gestiones simulan el CRUD**

 **Primera parte**
 - 1 html5: estructura del login
 - 1.1 crear la estructura de software

**Registar**
<a href="registro.html">Registrarse</a>
<input type="email" id="correo" required>
- 1.2 creamos el index.thml que contiene el login
- 2 iniciamos con css que permite generar los estilos personalizados de la pagina con variables de marca, generales

**index inventario**
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Iniciar sesion Inventario ADSO</title>
</head>
<body>
    <main><!--Contenido principal de la pagina-->
        <header><!---encabezado de login-->
            <h1>Inventario Sena</h1>
            <p>Ingresa tus credenciales para continuar</p>
        </header>

        <form action="dashboard.html" method="get"><!--Form perimite crear el contenido de un formulario cuando se envia nos lleva a la ruta medhod nos envia la
         informacion con get-->
        <div><!--agrupar un contenido en un contenedor-->
            <label for="correo">Correo Electronico</label><!--es una etiqueta de texto que con el for conecta con el input-->
            <input type="email" id="correo" placeholder="sena@correo.com" required><!--type obliga que tenga el @, placeholder el texto de ejemplo required es que es un
             campo obligatorio-->
        </div><p></p>

        <div>
            <label for="clave">Contraseña</label>
            <input type="password" id="clave" placeholder="Minimo 6 caracteres" minlength="6" required><!--type=password oculta lo que escribes, minlength=6 exige al menos
             6 caracteres-->
        </div><p></p>

        <div>
           <input type="checkbox" id="recordar"><!--type checkbox es casilla de verificacion-->
           <label for="recordar">Recordarme</label>
        </div>
        <button type="submit">Ingresar</button><!--envia el formulario antes revisa loa campos required email y minlength-->
        </form><!--Cierra el formulario-->

        <p>¿No tienes cuenta?<a href="registro.html">Registratre</p>
        <foother> 2026 SENA - ADSO Mixto </footer><!--pie de pagina-->
    </main>
</body>
</html>

**estilos css**
