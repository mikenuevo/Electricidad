
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servicios Eléctricos Industriales</title>

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- Iconos de Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">

    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #6ab8b8;
        }

       header {
    background: linear-gradient(45deg, #0056a3);
    color: #000000;
    padding: 2rem 0;
    position: sticky;
    top: 0;
    z-index: 1000;
    text-align: center;
}

header h1, 
header h2, 
header h3 {
    color: #000000;
    text-shadow: 
        -1px -1px 0 #fff, 
        1px -1px 0 #fff,
        -1px 1px 0 #fff,
        1px 1px 0 #fff;
}



        .nav-link {
            color: white !important;
            font-weight: bold;
            transition: color 0.3s;
        }

        .nav-link:hover {
            color: #ffd700 !important;
        }

        .imagen-servicio {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s;
        }

        .imagen-servicio:hover {
            transform: scale(1.05);
        }

        .card {
            border: none;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        footer {
            background-color: #343a40;
            color: white;
            padding: 2rem 0;
        }

        .social-icon {
            font-size: 1.5rem;
            margin: 0 10px;
            color: white;
            transition: color 0.3s;
        }

        .social-icon:hover {
            color: #ffd700;
        }
    </style>
</head>

<body>
    <header class="text-center">
        <h1>Servicios Eléctricos Industriales en Guatemala</h1>
        <h3>Especialista en mantenimiento, instalaciones y diagnósticos eléctricos</h3>
        <nav class="mt-3">
            <a href="#servicios" class="btn btn-warning mx-2">Servicios</a>
            <a href="#contacto" class="btn btn-warning mx-2">Contacto</a>
        </nav>
    </header>

    <main class="container my-5">
        <!-- Sección de Servicios -->
        <section id="servicios" class="mb-5">
            <h2 class="text-center mb-4">Nuestros Servicios</h2>
            <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">
                <div class="col">
                    <div class="card h-100 text-center">
                        <img src="img/instalacion.jpg" alt="Instalación eléctrica" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Instalación Eléctrica Industrial</h5>
                            <p class="card-text">Precio estimado: Q800 - Q1500</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100 text-center">
                        <img src="img/mantenimiento.jpg" alt="Mantenimiento de motores" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Mantenimiento de Motores Eléctricos</h5>
                            <p class="card-text">Precio estimado: Q500 - Q1200</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100 text-center">
                        <img src="img/diagnostico.jpg" alt="Diagnóstico de fallas" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Diagnóstico de Fallas</h5>
                            <p class="card-text">Precio estimado: Q400 - Q700</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100 text-center">
                        <img src="img/reparaciones.jpg" alt="Reparaciones generales" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Reparaciones Generales</h5>
                            <p class="card-text">Precio estimado: Q300 - Q1000</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección de Contacto -->
        <section id="contacto" class="mb-5">
            <h2 class="text-center mb-4">Contáctanos</h2>
            <p class="text-center">EMERGENCIA LAS 24 HORAS</p>
            <form class="mx-auto" style="max-width: 600px;" onsubmit="sendToWhatsApp(event)">
                <div class="mb-3">
                    <label for="name" class="form-label">Nombre Completo</label>
                    <input type="text" id="name" class="form-control" placeholder="Tu nombre" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Correo Electrónico</label>
                    <input type="email" id="email" class="form-control" placeholder="Tu correo" required>
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Mensaje</label>
                    <textarea id="message" class="form-control" placeholder="Tu mensaje" rows="5" required></textarea>
                </div>
                <div class="text-center">
                    <button type="button" class="btn btn-light">Enviar</button>
                </div>
            </form>
        </section>
    </main>

    <!-- Pie de página -->
    <footer class="text-center">
        <p>&copy; 2024 Servicios Eléctricos Industriales. Todos los derechos reservados.</p>
        <p>Síguenos en nuestras redes sociales:</p>
        <a href="#" class="social-icon"><i class="bi bi-facebook"></i></a>
        <a href="#" class="social-icon"><i class="bi bi-instagram"></i></a>
        <a href="#" class="social-icon"><i class="bi bi-whatsapp"></i></a>
    </footer>

    <!-- Bootstrap JS Bundle -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

    <script>
        function sendToWhatsApp(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;

            const phoneNumber = "50256352393";
            const text = `Hola, soy ${name}, mi correo es ${email}. Este es mi mensaje: ${message}`;
            const url = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(text)}`;

            window.location.href = url;
        }
    </script>
</body>

</html>
