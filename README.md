<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Makeupkat - Tienda de Maquillaje</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fff0f5;
            color: #333;
            text-align: center;
        }
        header {
            background-color: #ff85a2;
            color: white;
            padding: 1rem;
        }
        header img.logo {
            max-width: 150px;
            height: auto;
            margin-bottom: 0.5rem;
        }
        header h1 {
            margin: 0;
            font-size: 1.8rem;
        }
        .hero {
            padding: 2rem;
            background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1522335786673-4a5d3a0e6d2e');
            background-size: cover;
            background-position:jó

System: center;
            color: white;
        }
        .hero h2 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }
        .hero .whatsapp-button {
            background-color: #25D366;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-size: 1rem;
            display: inline-block;
            margin: 1rem 0;
            transition: background-color 0.3s;
        }
        .hero .whatsapp-button:hover {
            background-color: #20b354;
        }
        .products {
            padding: 1rem;
        }
        .products h2 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: #ff85a2;
        }
        .product-card {
            background-color: white;
            border-radius: 8px;
            padding: 1rem;
            margin: 1rem auto;
            width: 90%;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .product-card img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
        .product-card h3 {
            font-size: 1.2rem;
            margin: 0.5rem 0;
        }
        .product-card p {
            font-size: 0.9rem;
            color: #666;
            margin-bottom: 1rem;
        }
        .product-card .whatsapp-button {
            background-color: #25D366;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-size: 1rem;
            transition: background-color 0.3s;
        }
        .product-card .whatsapp-button:hover {
            background-color: #20b354;
        }
        footer {
            background-color: #ff85a2;
            color: white;
            padding: 1rem;
            font-size: 0.9rem;
        }
        @media (min-width: 768px) {
            .product-card {
                width: 80%;
            }
            header img.logo {
                max-width: 200px;
            }
        }
    </style>
</head>
<body>
    <header>
        <!-- Reemplaza la URL del logo con la de tu propio logo -->
        <img src="https://images.unsplash.com/photo-1586348943528-f28c309f9490" alt="Makeupkat Logo" class="logo">
        <h1>Makeupkat</h1>
    </header>
    <section class="hero">
        <h2>¡Encuentra tu maquillaje ideal!</h2>
        <p>Explora nuestros productos y ordena fácilmente por WhatsApp.</p>
        <!-- Reemplaza +1234567890 con tu número de WhatsApp real -->
        <a href="https://wa.me/1234567890?text=¡Hola! Quiero más información sobre los productos de Makeupkat." class="whatsapp-button" target="_blank">Explorar Productos</a>
    </section>
    <section class="products">
        <h2>Nuestros Productos</h2>
        <div class="product-card">
            <!-- Reemplaza la URL de la imagen con la de tu producto -->
            <img src="https://images.unsplash.com/photo-1522335786673-4a5d3a0e6d2e" alt="Paleta de Sombras">
            <h3>Paleta de Sombras Glam</h3>
            <p>Colores vibrantes y duraderos para cualquier look. $24.99</p>
            <!-- Reemplaza +1234567890 con tu número de WhatsApp real -->
            <a href="https://wa.me/1234567890?text=¡Hola! Quiero ordenar la Paleta de Sombras Glam." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <!-- Reemplaza la URL de la imagen con la de tu producto -->
            <img src="https://images.unsplash.com/photo-1512496015850-c4f373a4f8e5" alt="Labial Mate">
            <h3>Labial Mate Velvet</h3>
            <p>Tonos intensos con acabado mate de larga duración. $15.99</p>
            <!-- Reemplaza +1234567890 con tu número de WhatsApp real -->
            <a href="https://wa.me/1234567890?text=¡Hola! Quiero ordenar el Labial Mate Velvet." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <!-- Reemplaza la URL de la imagen con la de tu producto -->
            <img src="https://images.unsplash.com/photo-1522098605473-4ea11c27d8a6" alt="Base de Maquillaje">
            <h3>Base de Maquillaje Perfect</h3>
            <p>Cobertura impecable para un acabado natural. $29.99</p>
            <!-- Reemplaza +1234567890 con tu número de WhatsApp real -->
            <a href="https://wa.me/1234567890?text=¡Hola! Quiero ordenar la Base de Maquillaje Perfect." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
    </section>
    <footer>
        <!-- Actualiza el número de contacto y el correo si es necesario -->
        <p>Contáctanos: +123 456 7890 | info@makeupkat.com</p>
        <p>© 2025 Makeupkat - Tienda de Maquillaje</p>
    </footer>
</body>
</html>
