<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Product Page</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <!-- Navigation Bar -->
        <nav class="navbar">
            <div class="logo">ShopEasy</div>
            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#">Shop</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Cart</a></li>
            </ul>
        </nav>

        <!-- Product Section -->
        <div class="product-container">
            <div class="product-image">
                <img src="./Stylish Sneakers.jpeg" alt="Product Image">
            </div>
            <div class="product-details">
                <h1 class="product-name">Stylish Sneakers</h1>
                <p class="product-description">Comfortable and trendy sneakers
                    perfect for any occasion. Made with premium materials to
                    ensure durability and style.</p>
                <p class="product-price">$49.99</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>
        </div>

        <!-- Customer Reviews Section -->
        <section class="reviews">
            <h2>Customer Reviews</h2>
            <div class="review">
                <p>"Amazing quality! Very comfortable and stylish. Highly recommend!"</p>
                <span>- Akshay Guha</span>
            </div>
            <div class="review">
                <p>"Great value for the price. Will definitely buy again."</p>
                <span>- Saket Kumar Chaudhary</span>
            </div>
        </section>

        <!-- Related Products Section -->
        <section class="related-products">
            <h2>Related Products</h2>
            <div class="related-items">
                <div class="related-item">
                    <img src="./Running Shoes.jpeg" alt="Related Product 1">
                    <p>Running Shoes</p>
                </div>
                <div class="related-item">
                    <img src="./Casual T-Shirt.jpeg" alt="Related Product 2">
                    <p>Casual T-Shirt</p>
                </div>
                <div class="related-item">
                    <img src="./Stylish Backpack.jpeg" alt="Related Product 3">
                    <p>Stylish Backpack</p>
                </div>
            </div>
        </section>
        <script src="script.js"></script>
    </body>
</html>



/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background: #f4f4f4;
  }
  
  /* Navbar */
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background: #333;
    color: #fff;
  }
  
  .navbar .logo {
    font-size: 1.5rem;
    font-weight: bold;
  }
  
  .navbar .nav-links {
    list-style: none;
    display: flex;
  }
  
  .navbar .nav-links li {
    margin: 0 1rem;
  }
  
  .navbar .nav-links a {
    color: #fff;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .navbar .nav-links a:hover {
    color: #ffd700;
  }
  
  /* Product Section */
  .product-container {
    display: flex;
    flex-wrap: wrap;
    max-width: 1200px;
    margin: 2rem auto;
    background: #fff;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  }
  
  .product-image img {
    max-width: 100%;
    border-radius: 10px;
  }
  
  .product-details {
    flex: 1;
    padding: 1rem;
  }
  
  .product-name {
    font-size: 2rem;
    margin-bottom: 0.5rem;
  }
  
  .product-description {
    margin: 1rem 0;
  }
  
  .product-price {
    font-size: 1.5rem;
    font-weight: bold;
    color: #28a745;
  }
  
  .add-to-cart {
    background: #333;
    color: #fff;
    padding: 0.8rem 1.5rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  
  .add-to-cart:hover {
    background: #444;
  }
  
  /* Reviews Section */
  .reviews {
    max-width: 1200px;
    margin: 2rem auto;
    background: #fff;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  }
  
  .reviews h2 {
    margin-bottom: 1rem;
  }
  
  .review {
    margin-bottom: 1rem;
  }
  
  .review p {
    margin-bottom: 0.5rem;
    font-style: italic;
  }
  
  .review span {
    font-size: 0.9rem;
    color: #555;
  }
  
  /* Related Products Section */
  .related-products {
    max-width: 1200px;
    margin: 2rem auto;
    padding: 1.5rem;
    text-align: center;
  }
  
  .related-products h2 {
    margin-bottom: 1rem;
  }
  
  .related-items {
    display: flex;
    justify-content: center;
    gap: 1rem;
  }
  
  .related-item {
    text-align: center;
  }
  
  .related-item img {
    width: 150px;
    height: 150px;
    border-radius: 10px;
  }
  
  .related-item p {
    margin-top: 0.5rem;
  }


  // Toggle Mobile Navigation Menu
document.querySelector('.menu-toggle').addEventListener('click', () => {
    const navLinks = document.querySelector('.nav-links');
    navLinks.classList.toggle('show');
  });
  
