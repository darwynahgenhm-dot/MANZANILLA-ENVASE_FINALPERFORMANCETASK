
<!DOCTYPE html>
<html>
<head>
    <title>DONUT Eats</title>

    <style>
        body {
            background-color: pink;
            font-family: Arial;
            text-align: center;
        }

        h1 {
            color: white;
        }

        nav {
            background-color: hotpink;
            padding: 15px;
        }

        nav a {
            color: white;
            margin: 10px;
            text-decoration: none;
        }

        section {
            background-color: white;
            margin: 20px;
            padding: 20px;
            border-radius: 10px;
        }

        button {
            background-color: hotpink;
            color: white;
            padding: 10px;
            border: none;
        }
    </style>
</head>

<body>

    <h1>DONUT Eats 🍩</h1>
    <p>Sweetness in Every Bite!</p>

    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
        <a href="#settings">Settings</a>
    </nav>

    <section id="home">
        <h2>Home</h2>
        <p>Welcome to DONUT Eats!</p>
        <p>We sell delicious and sweet donuts for everyone.</p>
    </section>

    <section id="menu">
        <h2>Our Menu</h2>

        <h3>Strawberry Donut</h3>
        <p>Price: ₱25 | Size: Medium | Stocks: 20</p>

        <h3>Chocolate Donut</h3>
        <p>Price: ₱25 | Size: Medium | Stocks: 20</p>

        <h3>Glazed Donut</h3>
        <p>Price: ₱20 | Size: Medium | Stocks: 15</p>

        <h3>Cookies & Cream</h3>
        <p>Price: ₱30 | Size: Large | Stocks: 10</p>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>DONUT Eats is a small business that sells 
        tasty and affordable donuts.</p>
        <p>Our goal is to make people happy with our donuts!</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>Facebook: DONUT Eats</p>
        <p>Email: donuteats@gmail.com</p>

        <h3>Order Here!</h3>

        <input type="text" id="name" placeholder="Your Name"><br><br>

        <select id="donut">
            <option>Strawberry Donut</option>
            <option>Chocolate Donut</option>
            <option>Glazed Donut</option>
            <option>Cookies & Cream</option>
        </select><br><br>

        <input type="number" id="quantity" placeholder="Quantity"><br><br>

        <button onclick="order()">Order Now</button>

        <p id="message"></p>
    </section>

    <section id="settings">
        <h2>Settings</h2>
        <button onclick="changeColor()">Change Color</button>
        <button onclick="resetColor()">Reset</button>
    </section>

    <script>
        function order() {
            var name = document.getElementById("name").value;
            var donut = document.getElementById("donut").value;
            var quantity = document.getElementById("quantity").value;

            document.getElementById("message").innerHTML =
            "Thank you " + name + "! You ordered " + quantity + " " + donut + ".";
        }

        function changeColor() {
            document.body.style.backgroundColor = "lightblue";
        }

        function resetColor() {
            document.body.style.backgroundColor = "pink";
        }
    </script>

</body>
</html>
