# Ex.07 Restaurant Website
## Date:

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
rest.html


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Gourmet Haven | Redefined Elegance</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet"/>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" />
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <nav>
    <div class="logo">Gourmet Haven</div>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#menu">Menu</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section id="home" class="hero">
    <div class="hero-text">
      <h1>Refined Dining, Elevated Taste</h1>
      <p>Experience gourmet cuisine curated with passion, served with elegance.</p>
      <a href="#menu">Explore Menu</a>
    </div>
   
  </section>

  <section id="menu" class="section">
    <div class="section-title">
      <h2>Chef’s Specials</h2>
    </div>
    <div class="menu-grid">
      <div class="menu-item">
        <img src="./sea.webp" />
        <div class="menu-item-content">
          <h3>Seared Duck Breast</h3>
          <p>With port wine glaze and seasonal root vegetables.</p>
          <div class="price">$34.00</div>
        </div>
      </div>
      <div class="menu-item">
        <img src="./grilled-octopus.jpg" />
        <div class="menu-item-content">
          <h3>Charred Octopus</h3>
          <p>With smoked paprika aioli and heirloom potato medley.</p>
          <div class="price">$29.00</div>
        </div>
      </div>
      <div class="menu-item">
        <img src="./easy-creme-brulee-3.jpg" />
        <div class="menu-item-content">
          <h3>Crème Brûlée</h3>
          <p>Classic French vanilla custard with caramelized top.</p>
          <div class="price">$11.00</div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact" class="section">
    <div class="section-title">
      <h2>Reserve a Table</h2>
    </div>
    <div class="contact">
      <div>
        <h3>Visit Us</h3>
        <p><i class="fas fa-map-marker-alt"></i> 456 Elegant Ave, Food City</p>
        <p><i class="fas fa-phone"></i> (555) 678-9012</p>
        <p><i class="fas fa-envelope"></i> contact@gourmethaven.com</p>
      </div>
      <div class="contact-form">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <input type="date" required>
        <input type="time" required>
        <textarea placeholder="Special Requests"></textarea>
        <button type="submit">Submit</button>
      </div>
    </div>
  </section>

  <footer>
    <div class="social-links">
      <a href="#"><i class="fab fa-facebook-f"></i></a>
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
    </div>
    <p>&copy; 2025 Gourmet Haven. All rights reserved.</p>
  </footer>

</body>
</html>

style.html

:root {
  --primary: #b71c1c;
  --background: #121212;
  --text: #f5f5f5;
  --accent: #ffc107;
  --card-bg: #1e1e1e;
  --gray: #9e9e9e;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}

body {
  background-color: var(--background);
  color: var(--text);
}

nav {
  position: sticky;
  top: 0;
  background: rgba(18, 18, 18, 0.95);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  z-index: 1000;
}

nav .logo {
  font-size: 1.8rem;
  font-weight: bold;
  color: var(--accent);
}

nav ul {
  display: flex;
  gap: 2rem;
  list-style: none;
}

nav ul a {
  text-decoration: none;
  color: var(--text);
  font-weight: 500;
  transition: color 0.3s;
}

nav ul a:hover {
  color: var(--accent);
}

.hero {
  display: flex;
  flex-direction: row;
  height: 100vh;
}

.hero-text, .hero-image {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem;
}

.hero-text {
  flex-direction: column;
  text-align: left;
}

.hero-text h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.hero-text p {
  font-size: 1.2rem;
  color: var(--gray);
  margin-bottom: 2rem;
}

.hero-text a {
  background: var(--primary);
  color: white;
  padding: 0.8rem 1.5rem;
  border-radius: 25px;
  text-decoration: none;
  transition: background 0.3s;
}

.hero-text a:hover {
  background: #8c0c0c;
}

.hero-image img {
  width: 90%;
  max-height: 600px;
  object-fit: cover;
  border-radius: 20px;
}

.section {
  padding: 5rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

.section-title {
  text-align: center;
  margin-bottom: 3rem;
}

.section-title h2 {
  font-size: 2.5rem;
  border-bottom: 3px solid var(--primary);
  display: inline-block;
  padding-bottom: 0.5rem;
}

.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.menu-item {
  background: var(--card-bg);
  border-radius: 10px;
  overflow: hidden;
  transition: transform 0.3s ease;
}

.menu-item:hover {
  transform: scale(1.03);
}

.menu-item img {
  width: 100%;
  height: 180px;
  object-fit: cover;
}

.menu-item-content {
  padding: 1.2rem;
}

.menu-item-content h3 {
  margin-bottom: 0.5rem;
}

.menu-item-content p {
  color: var(--gray);
  font-size: 0.95rem;
  margin-bottom: 1rem;
}

.price {
  font-weight: bold;
  color: var(--accent);
}

.contact {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  align-items: center;
}

.contact-form input, .contact-form textarea {
  width: 100%;
  padding: 0.75rem;
  margin-bottom: 1rem;
  border: none;
  border-radius: 5px;
  background: #2a2a2a;
  color: white;
}

.contact-form textarea {
  resize: vertical;
  height: 120px;
}

.contact-form button {
  background: var(--primary);
  border: none;
  padding: 0.75rem 1.5rem;
  color: white;
  border-radius: 25px;
  cursor: pointer;
  transition: background 0.3s;
}

.contact-form button:hover {
  background: #8c0c0c;
}

footer {
  background: #000;
  color: #ccc;
  text-align: center;
  padding: 2rem 1rem;
  margin-top: 3rem;
}

.social-links a {
  color: white;
  margin: 0 1rem;
  font-size: 1.5rem;
  transition: color 0.3s;
}

.social-links a:hover {
  color: var(--accent);
}

```

## OUTPUT:
![alt text](<Screenshot 2025-05-20 231731.png>)
![alt text](<Screenshot 2025-05-20 231742.png>)
![alt text](<Screenshot 2025-05-20 231754.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
