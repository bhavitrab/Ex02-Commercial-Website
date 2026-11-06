# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

<h1>index.html</h1>




```

<!DOCTYPE html>
<html>
<head>
    <title>SHOPORA - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>

<body>

    <!-- Navigation Bar -->
    <header>
        <h1 class="logo">SHOPORA</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
            <a href="#account">Account</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="hero">
        <div>
            <h1>Welcome to SHOPORA</h1>
            <h2>Discover Your Perfect Style!</h2>
            <p>Fashion, Lifestyle and Accessories at Best Prices.</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="products">
        <h1>Our Products</h1>
        <p>Explore Our Exclusive Collection</p>

        <div class="product-container">

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=500" alt="Sports Shoes">
                <h3>Sports Shoes</h3>
                <p>Comfortable and stylish shoes.</p>
                <h4>₹1,499</h4>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=500" alt="Handbag">
                <h3>Handbag</h3>
                <p>Elegant bags for everyday use.</p>
                <h4>₹999</h4>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=500" alt="Watch">
                <h3>Wrist Watch</h3>
                <p>Modern watches with premium style.</p>
                <h4>₹1,299</h4>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=500" alt="Headphones">
                <h3>Headphones</h3>
                <p>Enjoy music with clear sound.</p>
                <h4>₹1,799</h4>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h1>About Us</h1>
        <p>
            SHOPORA is an online shopping platform that
            provides quality products at affordable prices.
            Our goal is to make shopping simple, easy and
            enjoyable for everyone.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h1>Contact Us</h1>
        <p>Email: support@shopora.com</p>
        <p>Phone: +91 9876543210</p>
        <p>Address: Chennai, Tamil Nadu, India</p>
    </section>

    <!-- User Account -->
    <section id="account" class="account">
        <h1>User Account</h1>

        <form>
            <input type="text" placeholder="Enter Your Name">
            <input type="email" placeholder="Enter Your Email">
            <input type="password" placeholder="Enter Password">
            <button type="submit">Login</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <h2>SHOPORA</h2>

        <div class="social">
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.youtube.com/">YouTube</a>
        </div>

        <p>© 2026 SHOPORA. All Rights Reserved.</p>
        <p>Name: BHAVITRA.B</p>
        <p>Register Number: 212225040047</p>
    </footer>

</body>
</html>

```




<h1>style.css</h1>




```


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #f5f5f5;
    color: #333;
}

/* Navigation */
header {
    background: #172554;
    color: white;
    padding: 20px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

.logo {
    color: #facc15;
    font-size: 28px;
}

nav {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

nav a:hover {
    color: #facc15;
}

/* Home */
.hero {
    min-height: 420px;
    background:
    linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
    url("https://images.unsplash.com/photo-1441986300917-64674bd600d8?w=1400");

    background-size: cover;
    background-position: center;

    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    padding: 30px;
}

.hero h1 {
    font-size: 42px;
    margin-bottom: 15px;
}

.hero h2 {
    color: #facc15;
    margin-bottom: 15px;
}

.hero p {
    margin-bottom: 25px;
    font-size: 18px;
}

.btn {
    background: #facc15;
    color: #172554;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

.btn:hover {
    background: white;
}

/* Products */
.products {
    padding: 50px 30px;
    text-align: center;
}

.products h1 {
    color: #172554;
    font-size: 32px;
    margin-bottom: 10px;
}

.products > p {
    margin-bottom: 30px;
}

.product-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 25px;
}

.product-card {
    background: white;
    width: 250px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    transition: 0.3s;
}

.product-card:hover {
    transform: translateY(-8px);
}

.product-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.product-card h3 {
    color: #172554;
    margin: 12px 0;
}

.product-card p {
    margin-bottom: 10px;
}

.product-card h4 {
    color: #e11d48;
    margin-bottom: 12px;
}

button {
    background: #172554;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #facc15;
    color: #172554;
}

/* About */
.about {
    background: #e0e7ff;
    text-align: center;
    padding: 50px 30px;
}

.about h1 {
    color: #172554;
    margin-bottom: 20px;
}

.about p {
    max-width: 750px;
    margin: auto;
    line-height: 1.8;
}

/* Contact */
.contact {
    background: white;
    text-align: center;
    padding: 40px;
}

.contact h1 {
    color: #172554;
    margin-bottom: 20px;
}

.contact p {
    margin: 10px;
}

/* Account */
.account {
    background: #e0e7ff;
    padding: 40px 20px;
    text-align: center;
}

.account h1 {
    color: #172554;
    margin-bottom: 20px;
}

.account form {
    display: flex;
    flex-direction: column;
    max-width: 350px;
    gap: 15px;
    margin: auto;
}

.account input {
    padding: 12px;
    border: 1px solid #aaa;
    border-radius: 5px;
}

/* Footer */
footer {
    background: #172554;
    color: white;
    text-align: center;
    padding: 25px;
}

footer h2 {
    color: #facc15;
    margin-bottom: 15px;
}

.social {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-bottom: 15px;
}

.social a {
    color: white;
    text-decoration: none;
}

.social a:hover {
    color: #facc15;
}

footer p {
    margin: 8px;
}

/* Responsive Design */
@media (max-width: 600px) {

    header {
        flex-direction: column;
        gap: 20px;
    }

    nav {
        justify-content: center;
        gap: 15px;
    }

    .hero h1 {
        font-size: 30px;
    }

    .product-card {
        width: 100%;
        max-width: 350px;
    }

    .social {
        flex-wrap: wrap;
    }
}

```

## OUTPUT
![alt text](<Screenshot 2026-11-06 083130.png>) ![alt text](<Screenshot 2026-11-06 083150.png>) ![alt text](<Screenshot 2026-11-06 083206.png>) ![alt text](<Screenshot 2026-11-06 083229.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
