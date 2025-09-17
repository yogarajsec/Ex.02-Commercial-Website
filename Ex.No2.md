# Ex02 Commercial Website
## Date:11/09/2025

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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px 15px;
        }
        nav a:hover {
            background-color: #555;
            border-radius: 5px;
        }
        .hero {
            display: flex;
            align-items: center;
            justify-content: center;
            background: url('realestate-hero.jpg') no-repeat center center/cover;
            height: 400px;
            color: white;
            text-align: center;
        }
        .hero h1 {
            font-size: 3rem;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
        }
        .properties {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
            gap: 20px;
        }
        .property {
            border: 1px solid #ddd;
            border-radius: 5px;
            overflow: hidden;
            width: 300px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .property img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .property-details {
            padding: 15px;
        }
        .property-details h3 {
            margin: 0 0 10px;
        }
        .property-details p {
            margin: 0 0 15px;
            color: #555;
        }
        .property-details a {
            text-decoration: none;
            color: white;
            background-color: #007BFF;
            padding: 10px 15px;
            border-radius: 5px;
        }
        .property-details a:hover {
            background-color: #0056b3;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Dream Homes Real Estate</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#properties">Properties</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="home" class="home">
        <div style="text-align: center; padding: 50px;">
            <h2>Welcome to Dream Homes Real Estate</h2>
            <p>We specialize in connecting you with your dream home. Whether you're looking for a luxury villa, a modern apartment, or a cozy cottage, we have the perfect property for you.</p>
            <a href="#properties" style="text-decoration: none; color: white; background-color: #007BFF; padding: 10px 20px; border-radius: 5px;">Browse Properties</a>
        </div>
    </section>
    <section class="hero">
        <h1>Find Your Dream Home Today</h1>
    </section>
    <section id="properties" class="properties">
        <div class="property">
            <img src="C:\Users\syoga\html\p1.png" alt="House 1">
            <div class="property-details">
                <h3>Luxury Villa</h3>
                <p>RS 1,200,000 - 4 Beds, 3 Baths</p>
                <a href="#">View Details</a>
            </div>
        </div>
        <div class="property">
            <img src="C:\Users\syoga\html\p2.png" alt="House 2">
            <div class="property-details">
                <h3>Modern Apartment</h3>
                <p>RS 850,000 - 3 Beds, 2 Baths</p>
                <a href="#">View Details</a>
            </div>
        </div>
        <div class="property">
            <img src="C:\Users\syoga\html\p3.png" alt="House 3">
            <div class="property-details">
                <h3>Cozy Cottage</h3>
                <p>RS 450,000 - 2 Beds, 1 Bath</p>
                <a href="#">View Details</a>
            </div>
        </div>
    </section>
    <section id="about" class="about" style="background-color: #f9f9f9; padding: 50px;">
        <div style="max-width: 800px; margin: auto; text-align: center;">
            <h2>About Us</h2>
            <p>Dream Homes Real Estate has been helping families find their perfect homes for over a decade. Our team of experienced agents is dedicated to providing exceptional service and ensuring a smooth buying or renting process. We pride ourselves on offering a wide range of properties to suit every lifestyle and budget.</p>
            <p>Our mission is to make your dream of owning a home a reality.</p>
        </div>
    </section>
    <section id="contact" class="contact" style="padding: 50px;">
        <div style="max-width: 600px; margin: auto; text-align: center;">
            <h2>Contact Us</h2>
            <p>Have questions or need assistance? We're here to help!</p>
            <p>Email: <a href="mailto:info@dreamhomes.com">info@dreamhomes.com</a></p>
            <p>Phone: <a href="tel:+1234567890">+91 2356789100</a></p>
            <p>Address: 123 Dream Street, Real Estate City, chennai</p>
            <form style="margin-top: 20px;">
                <input type="text" placeholder="Your Name" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <input type="email" placeholder="Your Email" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <textarea placeholder="Your Message" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;"></textarea>
                <button type="submit" style="background-color: #007BFF; color: white; padding: 10px 20px; border: none; border-radius: 5px;">Send Message</button>
            </form>
        </div>
    </section>
    <footer>
        <p>&copy; 2023 Dream Homes Real Estate. All rights reserved.</p>
    </footer>
</body>
</html>
```

## OUTPUT
<img width="1920" height="1080" alt="Screenshot 2025-09-17 151547" src="https://github.com/user-attachments/assets/82d999f3-5559-4c72-9657-cbc3a0f2c741" />
<img width="1920" height="1080" alt="Screenshot 2025-09-17 151602" src="https://github.com/user-attachments/assets/650ae4c3-1d63-4f33-b9a7-fae619249fdd" />
<img width="1920" height="1080" alt="Screenshot 2025-09-17 151609" src="https://github.com/user-attachments/assets/8068c9c9-5e5e-487e-94bb-e325684da78c" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
