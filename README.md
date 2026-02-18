<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Página de inicio de sesión con Bootstrap 5" />
    <title>CERTUS - Inicio de Sesión</title>
    
    <!-- ✅ BOOTSTRADP CSS desde CDN (web) -->
    <!-- Esta es la forma correcta de incluir Bootstrap desde internet -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    
    <!-- Estilos personalizados mínimos -->
    <style>
        /* Solo lo necesario para centrar el formulario */
        .form-signin {
            max-width: 330px;
            padding: 1rem;
        }
        
        /* Ajuste para el logo */
        .bd-placeholder-img {
            font-size: 1.125rem;
            text-anchor: middle;
            -webkit-user-select: none;
            -moz-user-select: none;
            user-select: none;
        }
        
        @media (min-width: 768px) {
            .bd-placeholder-img-lg {
                font-size: 3.5rem;
            }
        }
    </style>
</head>
<body class="d-flex align-items-center py-4 bg-body-tertiary">

    <!-- Contenido principal -->
    <main class="form-signin w-100 m-auto">
        <form>
            <!-- Logo (ahora usamos un texto en lugar de imagen local) -->
            <div class="text-center mb-4">
                <span class="fs-1 fw-bold text-primary">CERTUS</span>
            </div>
            
            <h1 class="h3 mb-3 fw-normal text-center">Inicie sesión</h1>

            <!-- Campo de email con floating labels -->
            <div class="form-floating mb-3">
                <input
                    type="email"
                    class="form-control"
                    id="floatingInput"
                    placeholder="nombre@ejemplo.com"
                    required
                />
                <label for="floatingInput">Correo electrónico</label>
            </div>

            <!-- Campo de contraseña con floating labels -->
            <div class="form-floating mb-3">
                <input
                    type="password"
                    class="form-control"
                    id="floatingPassword"
                    placeholder="Contraseña"
                    required
                />
                <label for="floatingPassword">Contraseña</label>
            </div>

            <!-- Checkbox Recuérdame -->
            <div class="form-check text-start my-3">
                <input
                    class="form-check-input"
                    type="checkbox"
                    value="remember-me"
                    id="checkDefault"
                />
                <label class="form-check-label" for="checkDefault">
                    Recuérdame
                </label>
            </div>

            <!-- Botón de ingreso -->
            <button class="btn btn-primary w-100 py-2" type="submit">
                Ingresar
            </button>

            <!-- Footer con copyright -->
            <p class="mt-5 mb-3 text-body-secondary text-center">&copy; 2024</p>
        </form>
    </main>

    <!-- ✅ BOOTSTRAP JavaScript desde CDN (web) -->
    <!-- Este script habilita los componentes interactivos de Bootstrap -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
    
    <!-- Script simple para redirección (opcional) -->
    <script>
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            // Aquí puedes poner la lógica de validación
            // Por ahora solo redirige a menu.html
            window.location.href = 'menu.html';
        });
    </script>
</body>
</html>
