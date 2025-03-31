# pizza-order-project-1
First attempt  at doing a pizza order page to see if I got it 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Pizza Project </title>
    <style>
body {
    font-family: Arial, sans-serif;
    margin: 20px;
    padding: 0;
}
body, html {
    height: 100 %;
}
body, h1, h2, h3, h4, h5, h6 {
    font-family: "Amatic SC", sans-serif;
}
.menu {
    display: none;
}
.bgimg {
    background-repeat: no-repeat;
    background-size: cover;
    background-image: URL("/w3images/pizza.jpg");
    min-height: 90 %;
}
        .container {
            max-width: 600 px;
            margin: 0 auto;
        }
        h1 {
            text-align: center;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-top: 10 px;
        }
        input, select, button {
            margin-top: 5 px;
            padding: 10 px;
            font-size: 16 px;
        }
        button {
            background-color: #00c0bc;
            Color: RGB(40, 14, 14);
            border: none;
            cursor: pointer;
        }
        button: hover {
            background-color: #217288;
        }
    </style>
</head>
body, html {height: 100%}
body,h1,h2,h3,h4,h5,h6 {font-family: "Amatic SC", sans-serif}
.menu {display: none}
.bgimg {
  background-repeat: no-repeat;
  background-size: cover;
  background-image: URL("/w3images/pizza.jpg");
  min-height: 90%;
}
</style>
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 0;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        h1 {
            text-align: center;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-top: 10px;
        }
        input, select, button {
            margin-top: 5px;
            padding: 10px;
            font-size: 16px;
        }
        button {
            background-color: #00c0bc;
            Color: RGB(40, 14, 14);
            border: none;
            cursor: pointer;
        }
        button: hover {
            background-color: #217288;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Order Your Pizza</h1>
        <form id="pizzaOrderForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="size">Pizza Size:</label>
            <select id="size" name="size" required>
                <option value="small">Small</option>
                <option value="medium">Medium</option>
                <option value="large">Large</option>
            </select>

            <label for="toppings">Toppings:</label>
            <select id="toppings" name="toppings" multiple>
                <option value="pepperoni">Pepperoni</option>
                <option value="mushrooms">Mushrooms</option>
                <option value="onions">Onions</option>
                <option value="sausage">Sausage</option>
                <option value="bacon">Bacon</option>
                <option value="extra_cheese">Extra Cheese</option>
                <option value="black_olives">Black Olives</option>
                <option value="green_peppers">Green Peppers</option>
            </select>

            <label for="instructions">Special Instructions:</label>
            <textarea id="instructions" name="instructions" rows="4"></textarea>

            <button type="submit">Place Order</button>
        </form>
    </div>

    <script>
        document.getElementById('pizzaOrderForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            const size = document.getElementById('size').value;
            const toppings = Array.from(document.getElementById('toppings').selectedOptions).map(option => option.value);
            const instructions = document.getElementById('instructions').value;

            alert(`Thank you, ${name}! Your ${size} pizza with ${toppings.join(', ')} is on its way!`);
        });
    </script>
</body>
</html>
}
body, h1, h2, h3, h4, h5, h6 {
    font-family: "Amatic SC", sans-serif;
}
.menu {
    display: none;
}
.bgimg {
    background-repeat: no-repeat;
    background-size: cover;
    background-image: URL("/w3images/pizza.jpg");
    min-height: 90%;
}
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        h1 {
            text-align: center;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-top: 10px;
        }
        input, select, button {
            margin-top: 5px;
            padding: 10px;
            font-size: 16px;
        }
        button {
            background-color: #00c0bc;
            color: RGB(40, 14, 14);
            border: none;
            cursor: pointer;
        }
        button: hover {
            background-color: #217288;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Order Your Pizza</h1>
        <form id="pizzaOrderForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="size">Pizza Size:</label>
            <select id="size" name="size" required>
                <option value="small">Small</option>
                <option value="medium">Medium</option>
                <option value="large">Large</option>
            </select>

            <label for="toppings">Toppings:</label>
            <select id="toppings" name="toppings" multiple>
                <option value="pepperoni">Pepperoni</option>
                <option value="mushrooms">Mushrooms</option>
                <option value="onions">Onions</option>
                <option value="sausage">Sausage</option>
                <option value="bacon">Bacon</option>
                <option value="extra_cheese">Extra Cheese</option>
                <option value="black_olives">Black Olives</option>
                <option value="green_peppers">Green Peppers</option>
            </select>

            <label for="instructions">Special Instructions:</label>
            <textarea id="instructions" name="instructions" rows="4"></textarea>

            <button type="submit">Place Order</button>
        </form>
    </div>

    <script>
        document.getElementById('pizzaOrderForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            const size = document.getElementById('size').value;
            const toppings = Array.from(document.getElementById('toppings').selectedOptions).map(option => option.value);
            const instructions = document.getElementById('instructions').value;

            alert(`Thank you, ${name}! Your ${size} pizza with ${toppings.join(', ')} is on its way!`);
        });
    </script>
</body>
</html>
