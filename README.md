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
            background-position: center;
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
        <img src="img/logo1.jpg" alt="Makeupkat Logo" class="logo">
        <h1>Makeupkat</h1>
    </header>
    <section class="hero">
        <h2>¡Encuentra tu maquillaje ideal!</h2>
        <p>Explora nuestros productos y ordena fácilmente por WhatsApp.</p>
        <a href="https://wa.me/+50249080900?text=¡Hola! Quiero más información sobre los productos de Makeupkat." class="whatsapp-button" target="_blank">Explorar Productos</a>
    </section>
    <section class="products">
        <h2>Nuestros Productos</h2>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1522335786673-4a5d3a0e6d2e" alt="Bálsamos Dupe de Dior en Barra">
            <h3>Bálsamos Dupe de Dior en Barra</h3>
            <p>Inspirados en el icónico Dior Lip Glow, estos bálsamos en barra ofrecen una hidratación profunda y un toque de color natural que realza el tono de tus labios. Formulados con ingredientes nutritivos como manteca de karité y aceites naturales, proporcionan suavidad y protección contra la resequedad.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar los Bálsamos Dupe de Dior en Barra." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1512496015850-c4f373a4f8e5" alt="Brillo Mágico de Fresita">
            <h3>Brillo Mágico de Fresita</h3>
            <p>El Brillo Mágico de Fresita es un labial cremoso con un delicioso aroma y sabor a fresa que aporta un brillo encantador. Su fórmula ligera y no pegajosa hidrata los labios mientras les da un tono rosado suave y natural.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Brillo Mágico de Fresita." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1522098605473-4ea11c27d8a6" alt="Bálsamo Hidratante de Fresita">
            <h3>Bálsamo Hidratante de Fresita</h3>
            <p>Este bálsamo labial con esencia de fresa combina hidratación intensiva con un delicado toque de color. Enriquecido con extractos de plantas y aceites naturales, previene el agrietamiento y mantiene los labios suaves y tersos durante todo el día.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Bálsamo Hidratante de Fresita." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1522335786673-4a5d3a0e6d2e" alt="Bálsamo Hidratante de Doble Fresita">
            <h3>Bálsamo Hidratante de Doble Fresita</h3>
            <p>El Bálsamo Hidratante de Doble Fresita ofrece el doble de hidratación y estilo en un solo producto. Con una fórmula enriquecida con manteca de karité y aceite de almendras, este bálsamo nutre profundamente los labios mientras los cubre con un brillo rosado.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Bálsamo Hidratante de Doble Fresita." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1512496015850-c4f373a4f8e5" alt="Bálsamo Hidratante de Vaselina (Rojo)">
            <h3>Bálsamo Hidratante de Vaselina (Rojo)</h3>
            <p>Este bálsamo labial de vaselina en tono rojo ofrece una hidratación duradera con un toque de color vibrante. Su fórmula clásica de vaselina protege los labios contra las agresiones externas, como el frío o el viento, mientras les da un acabado brillante.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Bálsamo Hidratante de Vaselina (Rojo)." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1522098605473-4ea11c27d8a6" alt="Bálsamo Hidratante de Vaselina (Azul)">
            <h3>Bálsamo Hidratante de Vaselina (Azul)</h3>
            <p>El Bálsamo Hidratante de Vaselina en tono azul combina la protección icónica de la vaselina con un sutil efecto refrescante. Su fórmula humectante mantiene los labios suaves y protegidos, mientras que su ligero tono azulado aporta un brillo único.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Bálsamo Hidratante de Vaselina (Azul)." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1522335786673-4a5d3a0e6d2e" alt="Bálsamo Hidratante de Vaselina (Café)">
            <h3>Bálsamo Hidratante de Vaselina (Café)</h3>
            <p>Con un cálido tono café, este bálsamo de vaselina hidrata profundamente y protege los labios mientras les da un acabado sofisticado y natural. Su fórmula enriquecida con ingredientes humectantes previene la resequedad y el agrietamiento.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Bálsamo Hidratante de Vaselina (Café)." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-152209860Occurrence: 1
5473-4ea11c27d8a6" alt="Antifaz de Animales">
            <h3>Antifaz de Animales</h3>
            <p>Los antifaces de animales son el accesorio perfecto para añadir diversión y estilo a cualquier ocasión. Disponibles en diseños adorables inspirados en animales, estos antifaces son ideales para fiestas, sesiones de fotos o simplemente para relajarte.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar el Antifaz de Animales." class="whatsapp-button" target="_blank">Ordenar</a>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1512496015850-c4f373a4f8e5" alt="Mascarillas para el Rostro">
            <h3>Mascarillas para el Rostro</h3>
            <p>Nuestras mascarillas faciales están diseñadas para hidratar, nutrir y revitalizar la piel. Formuladas con ingredientes naturales como extractos de frutas, ácido hialurónico y antioxidantes, ofrecen una experiencia de spa en casa.</p>
            <a href="https://wa.me/+50249080900?text=¡Hola! Quiero ordenar las Mascarillas para el Rostro." class="whatsapp-button" target="_blank">Ordenar</a>
            
