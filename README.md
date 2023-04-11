<!DOCTYPE html>

<html lang="en">
    <head>
        <!-- Meta Tag -->
        <meta charset="utf-8" />
        <meta name="viewport" content="initial-scale=1, width=device-width" />

        <!-- Custom CSS -->
        <link href="/static/css/styles.css" rel="stylesheet" />

        <!-- Bootstrap CSS & JS -->
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet">
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/js/bootstrap.bundle.min.js"></script>

        <!-- Bootstrap Icon -->
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css">

        <!-- Vertical Tab: https://github.com/tromgy/bootstrap-5-vertical-tabs -->
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-5-vertical-tabs@2.0.0/dist/b5vtabs.min.css"
        integrity="sha384-AsoWNxsuu73eGp2MPWHa77155fyqP9rueKOeG4t2d/AD4eyBqL20TClzfbAkrul4" crossorigin="anonymous" />

        <!-- Favicon -->
        <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
        <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
        <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
        <link rel="manifest" href="/static/favicon/site.webmanifest">
        <!-- Footer -->
        <script src="https://developer.edamam.com/attribution/badge.js"></script>

        <!-- Noto Emoji -->
        <link href='https://fonts.googleapis.com/css?family=Noto Emoji' rel='stylesheet'>

        <!-- Custom font -->
        <link rel="stylesheet" href="https://use.typekit.net/fet7rxe.css">

        <!-- jQuery -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

        <!-- Page Title -->
        <title>TasteTreatz | {% block title %}{% endblock %}</title>
    </head>

    <body>
        
        <!-- Header -->
        <!-- Header -->
        <nav class="navbar navbar-expand-md navbar-light">
            <!-- Title -->
            <div class="container py-3">
                <a href="/" class="navbar-brand">
                    <span class="playfair">TasteTreatz</span><br>
                </a>

                <!-- Navigation menu -->
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link custom-nav-link nav-item-animate" href="/">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link custom-nav-link" href="/about">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link custom-nav-link" href="/bookmarks">Bookmarks</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>


        <!-- Main -->
        <main class="container px-5">
            {% block main %}{% endblock %}
        </main>

        <!-- Footer -->
        <footer class="py-3">
            <div class="p-2 small mb-3 text-center">
            {% if session %}
            <!-- Edamam -->
            <div id="edamam-badge" data-color="badge"></div>
            <!-- Mockup Graphics -->
                <div class="small mb-3 text-muted">
                Photos by <a href="https://unsplash.com/@mockupgraphics?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText" target="_blank">Mockup Graphics</a> on <a href="https://unsplash.com/@mockupgraphics?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText" target="_blank">Unsplash</a>
                </div>
            {% endif %}
            <a href="https://github.com/Salima-Kh" target="_blank"><span class="p-2 footer text-muted bi bi-github"></span></a>
            </div>
        </footer>

        <!-- Script -->
        {% block script %}{% endblock %}
    </body>
</html>
