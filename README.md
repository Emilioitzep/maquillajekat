<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Makeupkat - Tienda y Gestión</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Roboto', sans-serif;
        }

        body {
            background: linear-gradient(to bottom, #fff0f5, #ffe6f0);
            min-height: 100vh;
        }

        header {
            background: linear-gradient(to right, #ff69b4, #ff85c0);
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header img {
            max-width: 150px;
            height: auto;
            margin-bottom: 0.5rem;
        }

        header h1 {
            font-size: 2rem;
            color: white;
        }

        .toggle-btn {
            position: fixed;
            top: 1rem;
            left: 1rem;
            background: #ff69b4;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .toggle-btn:hover, .toggle-btn:active {
            background: #e0559d;
            transform: scale(1.05);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        .login-section, .gestion-section, .tienda-section {
            display: none;
        }

        .login-section.active, .gestion-section.active, .tienda-section.active {
            display: block;
        }

        /* Estilos para Login */
        .login-section {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            max-width: 400px;
            margin: 3rem auto;
            text-align: center;
        }

        .login-section h2 {
            font-size: 1.5rem;
            color: #ff69b4;
            margin-bottom: 1rem;
        }

        .login-section input {
            width: 100%;
            padding: 0.8rem;
            margin: 0.5rem 0;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }

        .login-section button {
            width: 100%;
            padding: 0.8rem;
            background: #ff69b4;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .login-section button:hover, .login-section button:active {
            background: #e0559d;
            transform: scale(1.05);
        }

        /* Estilos para Gestión */
        .form-section {
            background: white;
            padding: 1.5rem;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            margin-bottom: 1.5rem;
        }

        .form-section input {
            width: 100%;
            padding: 0.8rem;
            margin: 0.5rem 0;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }

        .form-section button {
            width: 100%;
            padding: 0.8rem;
            background: #ff69b4;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .form-section button:hover, .form-section button:active {
            background: #e0559d;
            transform: scale(1.05);
        }

        .product-list {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .product-item {
            background: white;
            padding: 1rem;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .product-item img {
            width: 100px;
            height: 100px;
            object-fit: cover;
            border-radius: 8px;
        }

        .product-item div {
            flex-grow: 1;
        }

        .product-item h3 {
            color: #333;
            font-size: 1.2rem;
        }

        .product-item p {
            color: #666;
            font-size: 1rem;
        }

        .product-item button {
            background: #ff4444;
            color: white;
            border: none;
            padding: 0.6rem 1.2rem;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .product-item button:hover, .product-item button:active {
            background: #cc0000;
            transform: scale(1.05);
        }

        /* Estilos para Tienda */
        .productos {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 1.5rem;
            padding: 1rem;
        }

        .producto {
            background: white;
            padding: 1.5rem;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .producto:hover, .producto:active {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.15);
        }

        .producto img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 1rem;
        }

        .producto h3 {
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: #333;
        }

        .producto p {
            color: #666;
            font-size: 1rem;
            margin-bottom: 1rem;
        }

        .producto button {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .producto button:hover, .producto button:active {
            background: #e0559d;
            transform: scale(1.05);
        }

        .carrito {
            position: fixed;
            top: 1rem;
            right: 1rem;
            background: white;
            border: 1px solid #ddd;
            padding: 1.5rem;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            max-width: 300px;
        }

        .carrito h2 {
            font-size: 1.5rem;
            color: #ff69b4;
            margin-bottom: 1rem;
        }

        .carrito ul {
            list-style: none;
            padding: 0;
            margin-bottom: 1rem;
        }

        .carrito li {
            margin-bottom: 0.5rem;
            font-size: 1rem;
            color: #333;
        }

        .carrito p {
            font-size: 1.1rem;
            color: #333;
            margin-bottom: 1rem;
        }

        .carrito button {
            width: 100%;
            padding: 0.8rem;
            background: #ff69b4;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .carrito button:hover, .carrito button:active {
            background: #e0559d;
            transform: scale(1.05);
        }

        footer {
            background: #ff69b4;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

        footer p {
            font-size: 1rem;
        }

        footer a {
            color: #fff0f5;
            text-decoration: none;
            margin: 0 0.5rem;
        }

        footer a:hover {
            text-decoration: underline;
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 1.8rem;
            }

            header img {
                max-width: 120px;
            }

            .container {
                padding: 1rem 0.5rem;
            }

            .login-section {
                margin: 1rem;
                padding: 1.5rem;
            }

            .product-item {
                flex-direction: column;
                text-align: center;
            }

            .product-item img {
                width: 80px;
                height: 80px;
            }

            .productos {
                grid-template-columns: 1fr;
            }

            .producto img {
                height: 150px;
            }

            .carrito {
                position: fixed;
                bottom: 0;
                left: 0;
                right: 0;
                max-width: 100%;
                border-radius: 0;
                box-shadow: 0 -2px 5px rgba(0,0,0,0.1);
                padding: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="URL_DEL_LOGO_AQUÍ" alt="Makeupkat Logo">
        <h1>Makeupkat</h1>
    </header>

    <button class="toggle-btn" onclick="showLogin()">Ir a Gestión</button>

    <div class="container">
        <!-- Sección de Login -->
        <div class="login-section" id="loginSection">
            <h2>Iniciar Sesión</h2>
            <input type="password" id="passwordInput" placeholder="Contraseña">
            <button onclick="checkPassword()">Ingresar</button>
        </div>

        <!-- Sección de Gestión -->
        <div class="gestion-section" id="gestionSection">
            <h2>Gestión de Productos</h2>
            <div class="form-section">
                <input type="text" id="productName" placeholder="Nombre del producto">
                <input type="number" id="productPrice" placeholder="Precio (Q)" step="0.01">
                <input type="text" id="productImage" placeholder="URL de la imagen">
                <button onclick="addProduct()">Agregar Producto</button>
            </div>
            <div class="product-list" id="productList"></div>
        </div>

        <!-- Sección de Tienda -->
        <div class="tienda-section active" id="tiendaSection">
            <div class="productos" id="productGrid"></div>
        </div>
    </div>

    <div class="carrito" id="carrito">
        <h2>Carrito</h2>
        <ul id="listaCarrito"></ul>
        <p>Total: Q<span id="total">0</span></p>
        <button onclick="finalizarPedido()">Finalizar pedido</button>
    </div>

    <footer>
        <p>© 2025 Makeupkat. Todos los derechos reservados.</p>
        <p><a href="https://wa.me/50249080900"
