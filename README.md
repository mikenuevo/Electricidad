<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servicios Eléctricos Industriales</title>
    
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
        }

        header {
            background: #0077cc;
            color: white;
            padding: 1rem 0;
        }

        .imagen-servicio {
            width: 100%;
            height: 250px;
            object-fit: contain;
        }
    </style>
</head>

<body>
    <header class="text-center">
        <h1>Servicios Eléctricos Industriales en Guatemala</h1>
        <p>Especialista en mantenimiento, instalaciones y diagnósticos eléctricos</p>
        <nav class="my-3">
            <a href="#servicios" class="btn btn-outline-warning mx-2">Servicios</a>
            <a href="#contacto" class="btn btn-outline-warning mx-2">Contacto</a>
        </nav>
    </header>

    <main class="container my-5">
        <section id="servicios" class="mb-5">
            <h2 class="text-center mb-4">Servicios</h2>
            <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">
                <div class="col">
                    <div class="card h-100">
                        <img src="img/instalacion.jpg" alt="Instalación eléctrica" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Instalación Eléctrica Industrial</h5>
                            <p class="card-text">Precio estimado: Q800 - Q1500</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100">
                        <img src="img/mantenimiento.jpg" alt="Mantenimiento de motores" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Mantenimiento de Motores Eléctricos</h5>
                            <p class="card-text">Precio estimado: Q500 - Q1200</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100">
                        <img src="img/diagnostico.jpg" alt="Diagnóstico de fallas" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Diagnóstico de Fallas</h5>
                            <p class="card-text">Precio estimado: Q400 - Q700</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card h-100">
                        <img src="img/reparaciones.jpg" alt="Reparaciones generales" class="card-img-top imagen-servicio">
                        <div class="card-body">
                            <h5 class="card-title">Reparaciones Generales</h5>
                            <p class="card-text">Precio estimado: Q300 - Q1000</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contacto" class="mb-5">
            <h2 class="text-center mb-4">Contacto</h2>
            <p class="text-center">EMERGENCIA LAS 24 HORAS</p>
            <p class="text-center">Envíame tus consultas o solicita un presupuesto:</p>
            <form class="contact-form mx-auto" style="max-width: 600px;" onsubmit="sendToWhatsApp(event)">
                <div class="mb-3">
                    <input type="text" id="name" class="form-control" placeholder="Nombre completo" required>
                </div>
                <div class="mb-3">
                    <input type="email" id="email" class="form-control" placeholder="Correo electrónico" required>
                </div>
                <div class="mb-3">
                    <textarea id="message" class="form-control" placeholder="Escribe tu mensaje aquí" rows="5" required></textarea>
                </div>
                <div class="text-center">
                    <button type="submit" class="btn btn-primary">Enviar</button>
                </div>
            </form>
        </section>
    </main>

    <footer class="text-center py-3 bg-dark text-light">
        <p>&copy; 2024 Servicios Eléctricos Industriales - Todos los derechos reservados</p>
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
