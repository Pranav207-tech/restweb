# Ex.07 Restaurant Website
## Name:Pranav K
## Reg no:212224040240
## Date:26.05.25

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
home. html

<!DOCTYPE html>
<html lang="en">
<head>
    <title>Billal Restaurant</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            height: 100%;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: url('bg-billal.jpg') no-repeat center center fixed;
            background-size: cover;
            display: flex;
            flex-direction: column;
            position: relative;
        }

        .logo-bg {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            opacity: 0.08;
            z-index: 0;
            pointer-events: none;
        }

        .logo-bg img {
            max-width: 500px;
            width: 90%;
        }

        .container {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;
            background-color: rgba(255, 255, 255, 0.92);
            z-index: 1;
            position: relative;
        }

        .container h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #004d40;
        }

        .container p {
            font-size: 1.2rem;
            color: #444;
        }

        .button-group {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .btn {
            background-color: #00695c;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #00897b;
        }

        footer {
            text-align: center;
            padding: 15px;
            background-color: #f0f0f0;
            font-size: 0.9rem;
            color: #555;
        }
    </style>
</head>
<body>

    <!-- Logo as faint background -->
    <div class="logo-bg">
        <img src="billal-logo.png" alt="Billal Restaurant Logo">
    </div>

    <div class="container">
        <h1>Welcome to Billal Restaurant</h1>
        <p>Serving Tradition & Taste Since 1995</p>
        <div class="button-group">
            <a href="about.html" class="btn">About</a>
            <a href="menu.html" class="btn">Menu</a>
            <a href="contact.html" class="btn">Contact Us</a>
        </div>
    </div>

    <footer>
        Designed and Developed by Pranav K
    </footer>

</body>
</html>
```
```
about.html

<!DOCTYPE html>
<html lang="en">
<head>
  <title>About Us - Billal Restaurant</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      background-color: #fefefe;
      color: #333;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    header {
      background-color: #00695c;
      color: white;
      text-align: center;
      padding: 50px 20px 30px;
    }

    header h1 {
      font-size: 2.5rem;
    }

    header p {
      font-size: 1.1rem;
      margin-top: 10px;
    }

    .content {
      flex: 1;
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
      text-align: center;
    }

    .content h2 {
      font-size: 2rem;
      margin-bottom: 30px;
      color: #111;
    }

    .about-container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .about-text {
      text-align: justify;
      font-size: 1rem;
      max-width: 800px;
      margin-bottom: 30px;
    }

    .about-image {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    footer {
      background-color: #f8f9fa;
      padding: 15px;
      text-align: center;
      font-size: 0.9rem;
      color: #555;
    }

    @media (min-width: 768px) {
      .about-container {
        flex-direction: row;
        gap: 40px;
        justify-content: space-between;
      }

      .about-text {
        flex: 1;
      }

      .about-image {
        flex: 1;
        max-width: 400px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Our Culinary Journey</h1>
    <p>Authentic Flavors, Timeless Traditions</p>
  </header>

  <div class="content">
    <h2>About Us</h2>
    <div class="about-container">
      <div class="about-text">
        <p>
          Billal Restaurant was established in 1995 with the vision of bringing traditional, home-cooked flavors to a wider audience. Born in the heart of Tamil Nadu, our cuisine is deeply rooted in cultural heritage, using age-old family recipes and time-tested cooking techniques.
        </p>
        <p>
          Our dedication to quality and authenticity has earned us a loyal customer base over the years. Every dish we serve is crafted using fresh ingredients, select spices, and a deep respect for regional flavors — whether it's our signature biryani, aromatic curries, or sizzling grills.
        </p>
        <p>
          We believe that food is more than a meal — it is a memory in the making. At Billal Restaurant, we continue to serve our community with warmth, tradition, and a commitment to excellence that makes every visit unforgettable.
        </p>
      </div>
      <img src="images/images.jpg" alt="Billal Restaurant Founder" class="about-image"/>
    </div>
  </div>

  <footer>
    Designed and Developed by Pranav K
  </footer>

</body>
</html>
```
```
Menu.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Menu - Billal Restaurant</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #fff;
    }

    header {
      background-color: #00695c;
      color: white;
      padding: 1.5rem;
      text-align: center;
    }

    h2 {
      background-color: #00695c;
      color: white;
      padding: 1rem;
      text-align: center;
      margin: 2rem 0 1rem;
    }

    .menu-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
      padding: 0 1rem 2rem;
    }

    .menu-item {
      background-color: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      width: 300px;
      text-align: center;
    }

    .menu-item img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .menu-item .name {
      font-weight: bold;
      padding: 0.5rem 0 0.3rem;
    }

    .menu-item .price {
      color: #00695c;
      font-size: 1rem;
      padding-bottom: 0.8rem;
    }

    footer {
      background-color: #f5f5f5;
      color: #555;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

  <header>
    <h1>Billal Restaurant Menu</h1>
  </header>

  <h2>Biriyani</h2>
  <div class="menu-grid">
    <div class="menu-item">
      <img src="images/cb.jpg" alt="Chicken 65 Biryani">
      <p class="name">Chicken 65 Biryani</p>
      <p class="price">₹220</p>
    </div>
    <div class="menu-item">
      <img src="images/mb.avif" alt="Mutton Biryani">
      <p class="name">Mutton Biryani</p>
      <p class="price">₹260</p>
    </div>
    <div class="menu-item">
      <img src="images/ku.avif" alt="Kuska Biryani">
      <p class="name">Kuska</p>
      <p class="price">₹120</p>
    </div>
  </div>

  <h2>Starters</h2>
  <div class="menu-grid">
    <div class="menu-item">
      <img src="images/lol.jpg" alt="Chicken Lollipop">
      <p class="name">Chicken Lollipop</p>
      <p class="price">₹180</p>
    </div>
    <div class="menu-item">
      <img src="images/fish.jpg" alt="Fish Fry">
      <p class="name">Fish Fry</p>
      <p class="price">₹220</p>
    </div>
    <div class="menu-item">
      <img src="images/vm.jpg" alt="Veg Manchurian">
      <p class="name">Veg Manchurian</p>
      <p class="price">₹150</p>
    </div>
  </div>

  <h2>Sides</h2>
  <div class="menu-grid">
    <div class="menu-item">
      <img src="images/rai.jpg" alt="Raita">
      <p class="name">Raita</p>
      <p class="price">₹30</p>
    </div>
    <div class="menu-item">
      <img src="images/be.jpg" alt="Boiled Egg">
      <p class="name">Boiled Egg</p>
      <p class="price">₹20</p>
    </div>
    <div class="menu-item">
      <img src="images/pickle.jpg" alt="Pickle">
      <p class="name">Pickle</p>
      <p class="price">₹15</p>
    </div>
  </div>

  <h2>Gravy</h2>
  <div class="menu-grid">
    <div class="menu-item">
      <img src="images/nk.jpg" alt="Nalli Chops Kulambu">
      <p class="name">Nalli Chops Kulambu</p>
      <p class="price">₹180</p>
    </div>
    <div class="menu-item">
      <img src="images/pra.webp" alt="Chilli Prawns">
      <p class="name">Chilli Prawns</p>
      <p class="price">₹200</p>
    </div>
    <div class="menu-item">
      <img src="images/kc.jpg" alt="Kodaikanal Chicken">
      <p class="name">Kodaikanal Chicken</p>
      <p class="price">₹190</p>
    </div>
  </div>

  <h2>Desserts</h2>
  <div class="menu-grid">
    <div class="menu-item">
      <img src="images/jammu.jpg" alt="Gulab Jamun">
      <p class="name">Gulab Jamun (2 pcs)</p>
      <p class="price">₹60</p>
    </div>
    <div class="menu-item">
      <img src="images/pk.jpg" alt="Kesari">
      <p class="name">Pineapple Kesari</p>
      <p class="price">₹50</p>
    </div>
    <div class="menu-item">
      <img src="images/ep.jpg" alt="Elaneer Payasam">
      <p class="name">Elaneer Payasam</p>
      <p class="price">₹80</p>
    </div>
  </div>

  <footer>
    &copy; 2025 Billal Restaurant. All rights reserved.<br>
    Designed and Developed by Pranav K
  </footer>

</body>
</html>
```
```
contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Contact Us - Billal Restaurant</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f9f9f9;
      color: #333;
    }

    header {
      background-color: #00695c;
      color: white;
      padding: 1rem;
      text-align: center;
    }

    .container {
      max-width: 800px;
      margin: 2rem auto;
      padding: 1rem;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    h2 {
      color: #00695c;
    }

    .contact-info {
      margin-bottom: 2rem;
    }

    .contact-info p {
      margin: 0.5rem 0;
    }

    form {
      display: flex;
      flex-direction: column;
    }

    label {
      margin: 0.5rem 0 0.2rem;
    }

    input, textarea {
      padding: 0.6rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 1rem;
    }

    textarea {
      resize: vertical;
    }

    button {
      margin-top: 1rem;
      background-color: #00695c;
      color: white;
      padding: 0.7rem;
      border: none;
      border-radius: 4px;
      font-size: 1rem;
      cursor: pointer;
    }

    button:hover {
      background-color: #004d40;
    }

    footer {
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
      background-color: #eee;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Contact Us</h1>
  </header>

  <div class="container">
    <section class="contact-info">
      <h2>Billal Restaurant</h2>
      <p><strong>Address:</strong> No. 12, Bazaar Street, Vaniyambadi, Tamil Nadu - 635751</p>
      <p><strong>Phone:</strong> +91 98765 43210</p>
      <p><strong>Email:</strong> contact@billalrestaurant.com</p>
      <p><strong>Hours:</strong> 11:00 AM - 11:00 PM, All Days</p>
    </section>

    <section class="feedback-form">
      <h2>Send Us Your Feedback</h2>
      <form action="#" method="POST">
        <label for="name">Your Name</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Your Email</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Your Feedback</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <button type="submit">Submit Feedback</button>
      </form>
    </section>
  </div>

  <footer>
    &copy; 2025 Billal Restaurant. All rights reserved.<br>
    Designed and Developed by Pranav K
  </footer>
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2025-05-26 103322.png>)

![alt text](<Screenshot 2025-05-26 103337.png>)

![alt text](<Screenshot 2025-05-26 103355.png>)

![alt text](<Screenshot 2025-05-26 103407.png>)

![alt text](<Screenshot 2025-05-26 103424.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
