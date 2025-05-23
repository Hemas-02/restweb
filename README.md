# Ex.07 Restaurant Website
## Date:23/05/2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pizza Hut Express</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f5fff6;
      color: #2c2c2c;
    }

    header {
      position: sticky;
      top: 0;
      background-color: #6700e4;
      z-index: 10;
      text-align: center;
      padding: 10px 0;
    }

    .banner {
      width: 100%;
      height: 200px;
      object-fit: cover;
      display: block;
      margin-bottom: 10px;
    }

    nav ul {
      list-style: none;
      background-color: #bb1e10;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
    }

    nav ul li a {
      display: block;
      padding: 15px 20px;
      color: white;
      text-decoration: none;
    }

    nav ul li a:hover,
    nav ul li a.active {
      background-color: #7f0f08;
    }

    section {
      padding: 30px 20px;
      display: none;
    }

    section.active {
      display: block;
    }

    .menu-grid,
    .staff-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }

    .menu-item,
    .staff-member {
      background-color: #ffe1e1;
      padding: 15px;
      border: 1px solid #ddd;
      text-align: center;
    }

    .menu-item img,
    .staff-member img {
      width: 100%;
      height: 150px;
      object-fit: cover;
    }

    .intro {
      text-align: center;
    }

    footer {
      background-color: #111;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>
  <header>
    <img src="pizza banner.jpg" alt="Pizza Banner" class="banner" />
    <h1 style="color:white;">Pizza Hut Express</h1>
    <nav>
      <ul>
        <li><a href="#" class="nav-link active" data-target="home">Home</a></li>
        <li><a href="#" class="nav-link" data-target="menu">Menu</a></li>
        <li><a href="#" class="nav-link" data-target="staff">Team</a></li>
        <li><a href="#" class="nav-link" data-target="contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="active">
    <div class="intro">
      <h2>Welcome to Pizza Hut Express!</h2>
      <p>Delicious, hot, and fresh pizza delivered right to your table. Your pizza cravings end here.</p>
    </div>
  </section>

  <section id="menu">
    <h2>Our Pizza Menu</h2>
    <div class="menu-grid">
      <div class="menu-item">
        <img src="item1.jpg" alt="Pepperoni Pizza" />
        <h3>Pepperoni Pizza</h3>
        <p>Loaded with spicy pepperoni and cheese.</p>
        <p>$12.99</p>
      </div>
      <div class="menu-item">
        <img src="item2.jpg" alt="Veggie Delight" />
        <h3>Veggie Delight</h3>
        <p>Tomatoes, onions, peppers, and olives.</p>
        <p>$11.99</p>
      </div>
      <div class="menu-item">
        <img src="item3.jpg" alt="Cheese Lovers" />
        <h3>Cheese Lovers</h3>
        <p>Triple cheese explosion.</p>
        <p>$10.99</p>
      </div>
      <div class="menu-item">
        <img src="item4.jpg" alt="BBQ Chicken Pizza" />
        <h3>BBQ Chicken</h3>
        <p>Grilled chicken and BBQ sauce.</p>
        <p>$13.49</p>
      </div>
      <div class="menu-item">
        <img src="" alt="Meat Lovers" />
        <h3>Meat Lovers</h3>
        <p>Beef, chicken, sausage, bacon.</p>
        <p>$14.99</p>
      </div>
      <div class="menu-item">
        <img src="item6.jpg" alt="Hawaiian Pizza" />
        <h3>Hawaiian Pizza</h3>
        <p>Pineapple and ham blend.</p>
        <p>$12.49</p>
      </div>
      <div class="menu-item">
        <img src="item7.jpg" alt="Garlic Bread" />
        <h3>Garlic Bread</h3>
        <p>With melted cheese.</p>
        <p>$4.99</p>
      </div>
      <div class="menu-item">
        <img src="item8.jpg" alt="Chocolate Lava Cake" />
        <h3>Chocolate Lava Cake</h3>
        <p>Hot dessert with rich chocolate.</p>
        <p>$5.49</p>
      </div>
    </div>
  </section>

  <section id="staff">
    <h2>Meet Our Team</h2>
    <div class="staff-grid">
      <div class="staff-member">
        <img src="staff1.jpg" alt="Head Chef" />
        <h3>Rajesh Kumar</h3>
        <p>Head Chef</p>
      </div>
      <div class="staff-member">
        <img src="staff2.jpg" alt="Manager" />
        <h3>Sneha Patel</h3>
        <p>Restaurant Manager</p>
      </div>
      <div class="staff-member">
        <img src="staff3.jpg" alt="Lead Waiter" />
        <h3>Mohammed Ali</h3>
        <p>Lead Waiter</p>
      </div>
      <div class="staff-member">
        <img src="staff4.jpg" alt="Cashier" />
        <h3>Priya Rani</h3>
        <p>Front Desk / Cashier</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p><strong>Location:</strong> 456 Pizza Lane, Slice City, PC 67890</p>
    <p><strong>Phone:</strong> +1 555-987-6543</p>
    <p><strong>Email:</strong> order@pizzahutexpress.com</p>
  </section>

  <footer>
    <p>Created by <strong>Hemalatha</strong> © 2025</p>
  </footer>

  <script>
    const links = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('section');

    links.forEach(link => {
      link.addEventListener('click', e => {
        e.preventDefault();
        links.forEach(l => l.classList.remove('active'));
        link.classList.add('active');
        sections.forEach(sec => {
          sec.classList.remove('active');
          if (sec.id === link.dataset.target) {
            sec.classList.add('active');
          }
        });
      });
    });
  </script>
</body>
</html>

```

## OUTPUT:
![alt text](<Screenshot (69).png>)
![alt text](<Screenshot (70).png>)
![alt text](<Screenshot (71).png>)
![alt text](<Screenshot (72).png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
