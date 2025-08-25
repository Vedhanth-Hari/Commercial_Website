# Ex02 Commercial Website
## Date:24/08/2025
## NAME: VEDHANTH HARI
## REG NO: 212224240181

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
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BookMate - Read Anywhere</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f9f9f9;
            color: #333;
        }

        
        header {
            background-color: #4a148c;
            color: white;
            padding: 15px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 1.5rem;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

       
        .hero {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            padding: 50px;
            background-color: #ede7f6;
            text-align: center;
        }

        .hero-text {
            flex: 1;
            min-width: 300px;
            padding: 20px;
        }

        .hero-text h2 {
            font-size: 2rem;
            margin-bottom: 15px;
        }

        .hero-text p {
            font-size: 1.1rem;
            margin-bottom: 20px;
        }

        .hero-text a {
            display: inline-block;
            padding: 10px 20px;
            background-color: #4a148c;
            color: white;
            border-radius: 5px;
            text-decoration: none;
        }

        .hero-image img {
            max-width: 350px;
            border-radius: 10px;
        }

        /* Features */
        .features {
            padding: 50px 20px;
            background-color: white;
            text-align: center;
        }

        .features h2 {
            margin-bottom: 30px;
        }

        .feature-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .feature {
            background-color: #f3e5f5;
            padding: 20px;
            border-radius: 10px;
            width: 250px;
        }


        .plan {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            width: 250px;
            border: 2px solid #4a148c;
        }

        .plan h3 {
            margin-bottom: 10px;
        }

        .plan p {
            margin: 10px 0;
        }

        .plan a {
            display: inline-block;
            padding: 10px 15px;
            background-color: #4a148c;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }

        
        .contact {
            padding: 50px 20px;
            text-align: center;
        }

        
        footer {
            background-color: #4a148c;
            color: white;
            text-align: center;
            padding: 15px;
        }
    </style>
</head>
<body>

    
    <header>
        <h1>BookMate</h1>
        <nav>
            <ul>
                <li><a href="#login">LogIn</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#recommendation">Recommendations</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    
    <section class="hero">
        <div class="hero-text">
            <h2>Books at your fingertips</h2>
            <p>BookMate lets you read, buy, and explore thousands of books from anywhere. Available on mobile, tablet, and web.</p>
            <a href="#">Download the App</a>
        </div>
        <div class="hero-image">
            <img src="Book.jpg" alt="Book App">
        </div>
    </section>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Features - BookMate</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f5f5f5;
      color: #333;
    }

    header {
      background: #4a148c;
      color: white;
      text-align: center;
      padding: 20px;
    }

    header h1 {
      margin: 0;
    }

    .features-container {
      max-width: 1100px;
      margin: 30px auto;
      padding: 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .feature-box {
      background: white;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      transition: transform 0.3s;
      text-align: center;
    }

    .feature-box:hover {
      transform: translateY(-6px);
    }

    .feature-box h2 {
      color: #4a148c;
      margin-bottom: 10px;
    }

    .feature-box p {
      font-size: 0.95rem;
      line-height: 1.5;
      color: #555;
    }

    footer {
      background: #4a148c;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <header>
    <h1>App Features</h1>
    <p>Why choose BookMate for your reading journey?</p>
  </header>

  <div class="features-container">
    <div class="feature-box">
      <h2>📚 Smart Recommendations</h2>
      <p>Get personalized book suggestions based on your reading history and preferences.</p>
    </div>

    <div class="feature-box">
      <h2>🔍 Advanced Search</h2>
      <p>Find books by title, author, or genre quickly with our powerful search system.</p>
    </div>

    <div class="feature-box">
      <h2>⭐ Ratings & Reviews</h2>
      <p>See what other readers think before picking your next book.</p>
    </div>

    <div class="feature-box">
      <h2>📖 Online Reading</h2>
      <p>Read eBooks directly in the app with customizable fonts and dark mode.</p>
    </div>

    <div class="feature-box">
      <h2>📂 Wishlist & Library</h2>
      <p>Save your favorite titles to your wishlist and track your personal library.</p>
    </div>

    <div class="feature-box">
      <h2>🌍 Community</h2>
      <p>Join discussions, share reviews, and connect with other book lovers worldwide.</p>
    </div>

    <div class="feature-box">
      <h2>🎧 Audiobook Support</h2>
      <p>Listen to audiobooks on the go with background play and offline mode.</p>
    </div>

    <div class="feature-box">
      <h2>💡 Daily Recommendations</h2>
      <p>Discover a new handpicked book every day to expand your reading list.</p>
    </div>
  </div>



</body>
</html>

    
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Book Recommendations</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f3f0ff;
      color: #333;
    }

    header {
      background: #4a148c;
      color: white;
      padding: 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
    }

    .recommend-container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 20px;
    }

    .book-grid {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .book-card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      width: 220px;
      padding: 15px;
      text-align: center;
      transition: transform 0.3s;
    }

    .book-card:hover {
      transform: translateY(-8px);
    }

    .book-card img {
      width: 150px;
      height: 220px;
      border-radius: 8px;
      margin-bottom: 15px;
    }

    .book-card h3 {
      font-size: 1.1rem;
      color: #4a148c;
      margin: 10px 0 5px;
    }

    .book-card p {
      font-size: 0.9rem;
      color: #555;
    }

    footer {
      background: #4a148c;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Recommended Books</h1>
    <p>Curated just for you </p>
  </header>

  <div class="recommend-container">
    <div class="book-grid">

      
      <div class="book-card">
        <img src="Twisted love.jpg" alt="Book 1">
        <h3>The Twisted series</h3>
        <p>Ana Haung</p>
        <p>A emotional romance series about love, heartbreak, and the dangerous secrets that threaten to tear relationships apart..</p>
      </div>

      
      <div class="book-card">
        <img src="White Nights.jpg" alt="Book 2">
        <h3>White Nights</h3>
        <p>Fyodor Dostoevsk</p>
        <p>“White Nights” by Dostoevsky is a poignant tale of loneliness, fleeting love, and unfulfilled dreams set against the backdrop of St. Petersburg’s summer nights.</p>
      </div>

      
      <div class="book-card">
        <img src="Atomic Habits.jpg" alt="Book 3">
        <h3>Atomic Habits</h3>
        <p>James Clear</p>
        <p>Build better habits and break bad ones with proven strategies.</p>
      </div>

      
      <div class="book-card">
        <img src="Harry potter.jpg" alt="Book 4">
        <h3>Harry Potter</h3>
        <p>J.K. Rowling</p>
        <p>A magical journey of friendship, bravery, and destiny.</p>
      </div>

    </div>
  </div>



<section class="contact" id="contact">
    <h2>Contact Us</h2>
    <div class="contact-info">
        <p>Email: <a href="mailto:bookmate@gmail.com">bookmate@gmail.com</a></p>
        <p>Phone: <a href="tel:9876854354">9876854354</a></p>
    </div>
</section>


<footer>
    <p>&copy; 2025 BookMate. All Rights Reserved.</p>
</footer>

<style>
.contact {
    padding: 50px 20px;
    text-align: center;
    background: #f3e5f5;
    color: #333;
}

.contact h2 {
    margin-bottom: 15px;
    color: #4a148c;
}

.contact-info p {
    margin: 8px 0;
    font-size: 1.1rem;
}

.contact a {
    color: #4a148c;
    text-decoration: none;
    font-weight: bold;
}

.contact a:hover {
    text-decoration: underline;
}

footer {
    background: #4a148c;
    color: white;
    text-align: center;
    padding: 15px;
    margin-top: 20px;
}
</style>
```
login.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login | BookMate</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #4a148c, #7b1fa2);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .login-container {
      background: #fff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      width: 350px;
      text-align: center;
    }

    .login-container h2 {
      margin-bottom: 20px;
      color: #4a148c;
    }

    .login-container input {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 1rem;
    }

    .login-container button {
      width: 100%;
      padding: 12px;
      margin-top: 15px;
      background-color: #4a148c;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
    }

    .login-container button:hover {
      background-color: #6a1b9a;
    }

    .login-container p {
      margin-top: 15px;
      font-size: 0.9rem;
    }

    .login-container a {
      color: #4a148c;
      text-decoration: none;
      font-weight: bold;
    }

    .login-container a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  
  <div class="login-container">
    <h2>Login to BookMate</h2>
    <form>
      <input type="text" placeholder="Enter Email" required>
      <input type="password" placeholder="Enter Password" required>
      <button type="submit">Login</button>
    </form>
    <p>Don’t have an account? <a href="#">Sign Up</a></p>
  </div>

</body>
</html>
```

## OUTPUT
<img width="1871" height="1079" alt="Screenshot 2025-08-25 113205" src="https://github.com/user-attachments/assets/2c896500-4657-45f8-bcb4-5a5e0c29d77e" />
<img width="1869" height="1019" alt="Screenshot 2025-08-25 113241" src="https://github.com/user-attachments/assets/df324ead-9993-405b-be05-a1d4a1806885" />
<img width="1873" height="976" alt="Screenshot 2025-08-25 113339" src="https://github.com/user-attachments/assets/10e9d772-d298-4cf4-8ce6-64bae9fdb5b6" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
