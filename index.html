<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LUXE WEAR | Магазин стильной одежды</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&family=Playfair+Display:ital,wght@0,700;1,700&display=swap" rel="stylesheet">
    <style>
        /* ОСНОВНЫЕ СТИЛИ */
        :root {
            --black: #1a1a1a;
            --white: #ffffff;
            --gray: #f4f4f4;
            --accent: #c5a47e;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Montserrat', sans-serif; background-color: var(--white); color: var(--black); line-height: 1.6; }

        /* ШАПКА */
        header {
            padding: 30px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            background: rgba(255,255,255,0.95);
            z-index: 1000;
            border-bottom: 1px solid #eee;
        }

        .logo { font-family: 'Playfair Display', serif; font-size: 28px; font-weight: bold; letter-spacing: 2px; text-transform: uppercase; }

        nav a { margin-left: 30px; text-decoration: none; color: var(--black); font-size: 13px; text-transform: uppercase; letter-spacing: 1px; transition: 0.3s; }
        nav a:hover { color: var(--accent); }

        /* ГЛАВНЫЙ БАННЕР */
        .hero {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: var(--gray);
            margin-bottom: 50px;
        }

        .hero h1 { font-family: 'Playfair Display', serif; font-size: 60px; margin-bottom: 10px; }
        .hero p { text-transform: uppercase; letter-spacing: 3px; color: #777; }

        /* СЕТКА ТОВАРОВ */
        .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
        
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 40px;
            margin-bottom: 100px;
        }

        .product-card {
            position: relative;
            overflow: hidden;
            transition: 0.4s;
            cursor: pointer;
        }

        .product-image {
            width: 100%;
            height: 400px;
            background-size: cover;
            background-position: center;
            transition: 0.5s;
            background-color: #eee;
        }

        .product-card:hover .product-image { transform: scale(1.05); }

        .product-info { margin-top: 15px; text-align: center; }
        .product-title { font-size: 16px; font-weight: 400; text-transform: uppercase; margin-bottom: 5px; }
        .product-price { color: var(--accent); font-weight: 600; }

        /* ФОРМА ДОБАВЛЕНИЯ (АДМИНКА) */
        .admin-panel {
            background: var(--gray);
            padding: 50px 20px;
            margin-top: 50px;
            border-top: 2px solid var(--black);
        }

        .admin-panel h2 { text-align: center; margin-bottom: 30px; font-family: 'Playfair Display', serif; }

        .add-form {
            max-width: 500px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .add-form input {
            padding: 12px;
            border: 1px solid #ddd;
            font-family: inherit;
        }

        .add-form button {
            padding: 15px;
            background: var(--black);
            color: white;
            border: none;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: 0.3s;
        }

        .add-form button:hover { background: var(--accent); }

        footer { text-align: center; padding: 50px; font-size: 12px; color: #aaa; text-transform: uppercase; }

    </style>
</head>
<body>

    <header>
        <div class="logo">Luxe Wear</div>
        <nav>
            <a href="#">Новинки</a>
            <a href="#">Каталог</a>
            <a href="#">О нас</a>
            <a href="#">Корзина (0)</a>
        </nav>
    </header>

    <section class="hero">
        <p>Новая коллекция 2024</p>
        <h1>Эстетика Комфорта</h1>
    </section>

    <div class="container">
        <div class="products-grid" id="productsDisplay">
            <!-- Сюда будут добавляться товары -->
        </div>
    </div>

    <!-- АДМИН-ПАНЕЛЬ ДЛЯ ТЕБЯ -->
    <section class="admin-panel">
        <div class="container">
            <h2>Добавить новую одежду</h2>
            <div class="add-form">
                <input type="text" id="imgUrl" placeholder="Ссылка на фото (URL)">
                <input type="text" id="itemName" placeholder="Название товара">
                <input type="text" id="itemPrice" placeholder="Цена (например: 4 500 ₽)">
                <button onclick="addItem()">Опубликовать на сайт</button>
                <button onclick="clearItems()" style="background: #cc0000; margin-top: 10px;">Очистить всё</button>
            </div>
        </div>
    </section>

    <footer>
        &copy; 2024 Luxe Wear Studio. Все права защищены.
    </footer>

    <script>
        // Начальные товары, если список пуст
        const defaultProducts = [
            {
                name: "Шерстяное пальто",
                price: "12 900 ₽",
                image: "https://images.unsplash.com/photo-1539533377285-a9214197460c?auto=format&fit=crop&w=500&q=80"
            },
            {
                name: "Льняная рубашка",
                price: "4 200 ₽",
                image: "https://images.unsplash.com/photo-1596755094514-f87034a2612d?auto=format&fit=crop&w=500&q=80"
            }
        ];

        // Загрузка товаров из памяти браузера
        let products = JSON.parse(localStorage.getItem('myClothes')) || defaultProducts;

        // Функция отображения товаров
        function displayProducts() {
            const grid = document.getElementById('productsDisplay');
            grid.innerHTML = '';

            products.forEach(item => {
                grid.innerHTML += `
                    <div class="product-card">
                        <div class="product-image" style="background-image: url('${item.image}')"></div>
                        <div class="product-info">
                            <h3 class="product-title">${item.name}</h3>
                            <p class="product-price">${item.price}</p>
                        </div>
                    </div>
                `;
            });
        }

        // Функция добавления товара
        function addItem() {
            const name = document.getElementById('itemName').value;
            const price = document.getElementById('itemPrice').value;
            const image = document.getElementById('imgUrl').value;

            if(name && price && image) {
                products.push({name, price, image});
                localStorage.setItem('myClothes', JSON.stringify(products));
                displayProducts();
                
                // Очистка полей
                document.getElementById('itemName').value = '';
                document.getElementById('itemPrice').value = '';
                document.getElementById('imgUrl').value = '';
            } else {
                alert("Пожалуйста, заполни все поля!");
            }
        }

        // Удаление всех товаров
        function clearItems() {
            if(confirm("Удалить все товары?")) {
                localStorage.removeItem('myClothes');
                products = defaultProducts;
                displayProducts();
            }
        }

        // Запуск при загрузке
        displayProducts();
    </script>
</body>
</html>
