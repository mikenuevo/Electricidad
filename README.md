<!DOCTYPE html>

<html lang="es">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Servicios Eléctricos Industriales</title>

    <style>

        body {

            font-family: Arial, sans-serif;

            margin: 0;

            padding: 0;

            background-color: #f4f4f4;

            color: #333;

        }

        header {

            background: #0077cc;

            color: white;

            padding: 1rem 0;

            text-align: center;

        }

        nav {

            text-align: center;

            margin: 10px 0;

        }

        nav a {

            margin: 0 15px;

            text-decoration: none;

            color: white;

            font-weight: bold;

        }

        section {

            padding: 2rem;

            text-align: center;

        }

        .services {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

            gap: 15px;

        }

        .service {

            background: white;

            border: 1px solid #ddd;

            padding: 1rem;

            border-radius: 5px;

            text-align: center;

        }

        .service img {

            max-width: 100%;

            border-radius: 5px;

        }

        

        .contact-form input, .contact-form textarea {

            width: 100%;

            margin: 10px 0;

            padding: 10px;

            border: 1px solid #ddd;

            border-radius: 5px;

        }

        .contact-form button {

            background: #0077cc;

            color: white;

            padding: 10px 15px;

            border: none;

            border-radius: 5px;

            cursor: pointer;

        }



	

	img {

        width: 500px;

        height: auto;

        object-fit: cover; 

    	}



	.imagen-servicio {

        width: 250px;

        height: 250px;         

	object-fit: contain; 



	}

    </style>

</head>

<body>



<header>

    <h1>Servicios Eléctricos Industriales en Guatemala</h1>

    <p>Especialista en mantenimiento, instalaciones y diagnósticos eléctricos</p>

    <nav>

        <a href="#servicios">Servicios</a>

        <a href="#contacto">Contacto</a>

    </nav>

</header>



<section id="servicios">

    <h2>Servicios</h2>

    <div class="services">

        <div class="service">

            <img src="img\instalacion.jpg" alt="Instalación eléctrica" class="imagen-servicio">

            <h3>Instalación Eléctrica Industrial</h3>

            <p>Precio estimado: Q800 - Q1500</p>

        </div>

        <div class="service">

            <img src="img\mantenimiento.jpg" alt="Mantenimiento de motores" class="imagen-servicio">

            <h3>Mantenimiento de Motores Eléctricos</h3>

            <p>Precio estimado: Q500 - Q1200</p>

        </div>

        <div class="service">

            <img src="img\diagnostico.jpg" alt="Diagnóstico de fallas" class="imagen-servicio">

            <h3>Diagnóstico de Fallas</h3>

            <p>Precio estimado: Q400 - Q700</p>

        </div>

        <div class="service">

            <img src="img\reparaciones.jpg" alt="Reparaciones generales" class="imagen-servicio">

            <h3>Reparaciones Generales</h3>

            <p>Precio estimado: Q300 - Q1000</p>

        </div>

    </div>

</section>



<section id="contacto">

    <h2>Contacto</h2>

    <p>Envíame tus consultas o solicita un presupuesto:</p>

    <form class="contact-form" action="#" method="post">

        <input type="text" name="name" placeholder="Nombre completo" required>

        <input type="email" name="email" placeholder="Correo electrónico" required>

        <textarea name="message" placeholder="Escribe tu mensaje aquí" rows="5" required></textarea>

        <button type="submit">Enviar</button>

    </form>

</section>



<footer>

    <p>&copy; 2024 Servicios Eléctricos Industriales - Todos los derechos reservados</p>

</footer>



</body>

</html>
