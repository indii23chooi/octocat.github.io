<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sakura Sushi Bar</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            line-height: 1.6;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 1rem 0;
        }
        nav ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
        }
        .hero {
            background-image: url('hero.jpg');
            background-size: cover;
            background-position: center;
            height: 500px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #fff;
        }
        .hero h1 {
            font-size: 3rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        section {
            padding: 4rem 0;
        }
        h2 {
            text-align: center;
            margin-bottom: 2rem;
        }
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        .menu-item {
            border: 1px solid #ddd;
            padding: 1rem;
            text-align: center;
        }
        .menu-item img {
            max-width: 100%;
            height: auto;
        }
        .contact-info {
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h1>Welcome to Sakura Sushi Bar</h1>
        </div>
    </section>

    <section id="about">
        <div class="container">
            <h2>About Us</h2>
            <p>Sakura Sushi Bar offers the finest Japanese cuisine in town. Our expert chefs prepare fresh, delicious sushi and other Japanese delicacies using only the highest quality ingredients.</p>
        </div>
    </section>

    <section id="menu">
        <div class="container">
            <h2>Our Menu</h2>
            <div class="menu-grid">
                <div class="menu-item">
                    <img src="california.jpg" alt="California Roll">
                    <h3>California Roll</h3>
                    <p>RM 12.00</p>
                </div>
                <div class="menu-item">
                    <img src="salmon.jpg" alt="Salmon Nigiri">
                    <h3>Salmon Nigiri</h3>
                    <p>RM 8.00</p>
                </div>
                <div class="menu-item">
                    <img src="tuna.jpg" alt="Tuna Sashimi">
                    <h3>Tuna Sashimi</h3>
                    <p>RM 18.00</p>
                </div>
                <div class="menu-item">
                    <img src="tempura.jpg" alt="Veggie Tempura">
                    <h3>Veggie Tempura</h3>
                    <p>RM 9.00</p>
                </div>
                <div class="menu-item">
                    <img src="miso.jpg" alt="Miso Soup">
                    <h3>Miso Soup</h3>
                    <p>RM 4.00</p>
                </div>
                <div class="menu-item">
                    <img src="greentea.jpg" alt="Green Tea Ice Cream">
                    <h3>Green Tea Ice Cream</h3>
                    <p>RM 5.00</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <div class="contact-info">
                <p>Email: order@sakurasushi.com</p>
                <p>WhatsApp: 018-2777989</p>
            </div>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
