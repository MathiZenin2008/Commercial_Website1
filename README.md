# Ex02 Commercial Website
## Date:31-10-2026

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
HTML PROGRAM
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopEase - Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>ShopEase</h1>
        <p>Your One-Stop Shopping Destination</p>
    </header>

    <!-- Navigation Bar -->
    <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
        <a href="#account">My Account</a>
    </nav>

    <!-- Homepage -->
    <section id="home" class="hero">
        <h2>Welcome to ShopEase</h2>
        <p>Discover the latest smartphones and Apple products at affordable prices!</p>
        <a href="#products" class="btn">Shop Now</a>
    </section>

    <!-- Products Section -->
    <section id="products">
        <h2>Our Products</h2>

        <div class="container">

            <!-- Product 1 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\s24.jpeg" alt="Samsung Galaxy">
                <h3>Samsung Galaxy S24</h3>
                <p>Price: ₹55,000</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 2 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\i16.jpeg" alt="Apple iPhone">
                <h3>Apple iPhone 16</h3>
                <p>Price: ₹65,000</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 3 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\ipad.jpeg" alt="Apple iPad">
                <h3>Apple iPad</h3>
                <p>Price: ₹35,000</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 4 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\iwatch.jpeg" alt="Apple Watch">
                <h3>Apple Watch</h3>
                <p>Price: ₹25,000</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 5 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\air.jpeg" alt="Apple AirPods">
                <h3>Apple AirPods</h3>
                <p>Price: ₹15,000</p>
                <button>Buy Now</button>
            </div>

            <!-- Product 6 -->
            <div class="product">
                <img src="c:\Users\acer\Pictures\Temp\1plus.jpeg" alt="OnePlus Smartphone">
                <h3>OnePlus Smartphone</h3>
                <p>Price: ₹40,000</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <!-- About Us -->
    <section id="about">
        <h2>About Us</h2>
        <p>
            ShopEase is an online commercial shopping platform.
            We provide the latest smartphones and Apple products
            at affordable prices with a simple and convenient
            shopping experience.
        </p>
    </section>

    <!-- Contact Details -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@shopease.com</p>
        <p>Phone: +91 9876543210</p>
        <p>Address: Chennai, Tamil Nadu, India</p>
    </section>

    <!-- User Account -->
    <section id="account">
        <h2>User Account</h2>

        <form>
            <input type="text" placeholder="Enter Username" required>
            <input type="email" placeholder="Enter Email" required>
            <input type="password" placeholder="Enter Password" required>
            <button type="submit">Login</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>Follow Us</p>

        <div class="social">
            <a href="https://www.facebook.com">Facebook</a>
            <a href="https://www.instagram.com">Instagram</a>
            <a href="https://www.twitter.com">Twitter</a>
        </div>

        <p>&copy; 2026 ShopEase. All Rights Reserved.</p>
    </footer>

</body>
</html>

```
CSS PROGRAM
```
/* ===========================
   ShopEase Commercial Website
   =========================== */

/* Reset */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#f5f7fa;
    color:#333;
    line-height:1.6;
}

/* Header */
header{
    background:linear-gradient(135deg,#0f172a,#1e3a8a);
    color:white;
    text-align:center;
    padding:35px 20px;
}

header h1{
    font-size:42px;
    letter-spacing:2px;
}

header p{
    margin-top:10px;
    font-size:18px;
    color:#dbeafe;
}

/* Navigation */
nav{
    display:flex;
    justify-content:center;
    align-items:center;
    flex-wrap:wrap;
    gap:15px;
    background:#14243A;
    padding:15px;
    position:sticky;
    top:0;
    z-index:1000;
}

nav a{
    color:white;
    text-decoration:none;
    padding:10px 20px;
    border-radius:25px;
    transition:0.3s;
    font-weight:bold;
}

nav a:hover{
    background:#ff9800;
    color:white;
}

/* Sections */
section{
    padding:60px 20px;
}

section h2{
    text-align:center;
    color:#14243A;
    font-size:32px;
    margin-bottom:30px;
}

/* Hero Section */
.hero{
    background:linear-gradient(rgba(20,36,58,.75),rgba(20,36,58,.75)),
    url("https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?auto=format&fit=crop&w=1400&q=80");
    background-size:cover;
    background-position:center;
    color:white;
    text-align:center;
    padding:120px 20px;
}

.hero h2{
    color:white;
    font-size:45px;
    margin-bottom:20px;
}

.hero p{
    font-size:20px;
    margin-bottom:30px;
}

.btn{
    display:inline-block;
    background:#ff9800;
    color:white;
    text-decoration:none;
    padding:15px 35px;
    border-radius:30px;
    font-size:18px;
    transition:0.3s;
}

.btn:hover{
    background:#ff7a00;
    transform:scale(1.05);
}

/* Product Layout using Flexbox */
.container{
    display:flex;
    justify-content:center;
    align-items:stretch;
    flex-wrap:wrap;
    gap:30px;
}

/* Product Card */
.product{
    background:white;
    width:300px;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 8px 20px rgba(0,0,0,.12);
    transition:0.3s;
}

.product:hover{
    transform:translateY(-10px);
    box-shadow:0 12px 28px rgba(0,0,0,.18);
}

.product img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.product h3{
    text-align:center;
    margin:20px 0 10px;
    color:#14243A;
}

.product p{
    text-align:center;
    font-size:18px;
    font-weight:bold;
    color:#ff9800;
}

.product button{
    display:block;
    width:85%;
    margin:20px auto;
    padding:12px;
    border:none;
    border-radius:8px;
    background:#14243A;
    color:white;
    font-size:16px;
    cursor:pointer;
    transition:0.3s;
}

.product button:hover{
    background:#ff9800;
}

/* About & Contact */
#about,#contact{
    background:white;
    max-width:1000px;
    margin:30px auto;
    border-radius:15px;
    box-shadow:0 5px 15px rgba(0,0,0,.08);
    text-align:center;
}

#about p,#contact p{
    font-size:18px;
    margin:12px 20px;
}

/* User Account */
#account{
    background:#eef3f8;
}

#account form{
    max-width:420px;
    margin:auto;
    display:flex;
    flex-direction:column;
    gap:18px;
}

#account input{
    padding:14px;
    border:1px solid #ccc;
    border-radius:8px;
    font-size:16px;
}

#account input:focus{
    outline:none;
    border-color:#1e3a8a;
    box-shadow:0 0 8px rgba(30,58,138,.2);
}

#account button{
    padding:14px;
    border:none;
    border-radius:8px;
    background:#14243A;
    color:white;
    font-size:16px;
    cursor:pointer;
    transition:0.3s;
}

#account button:hover{
    background:#ff9800;
}

/* Footer */
footer{
    background:#14243A;
    color:white;
    text-align:center;
    padding:35px 20px;
}

footer p{
    margin:10px 0;
}

/* Social Links using Flexbox */
.social{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:20px;
    margin:20px 0;
}

.social a{
    color:#ff9800;
    text-decoration:none;
    font-weight:bold;
    transition:0.3s;
}

.social a:hover{
    color:white;
    transform:scale(1.1);
}

/* Responsive Design */
@media(max-width:768px){

    header h1{
        font-size:32px;
    }

    .hero h2{
        font-size:32px;
    }

    .hero p{
        font-size:18px;
    }

    nav{
        flex-direction:column;
    }

    .container{
        flex-direction:column;
        align-items:center;
    }

    .product{
        width:90%;
        max-width:350px;
    }
}
```
## OUTPUT
![alt text](image-1.png)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
