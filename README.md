<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Travel Agency</title>
  <link rel="stylesheet" href="landing.css">
  <link href="https://cdn.jsdelivr.net/npm/remixicon@4.5.0/fonts/remixicon.css" rel="stylesheet"/>
</head>
<body>

  <!-- Header Section -->
  <header class="hero">
    <nav class="navbar">
      <h1 class="logo">BOSE TRAVELS</h1>
      <ul class="nav-links">
        <li><a href="#">Home</a></li>
        <li><a href="#">Destinations</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
    <div class="hero-content">
      <h2>Your Dream Vacation Awaits</h2>
      <p>Discover beautiful destinations and unforgettable experiences with us.</p>
      <a href="#services" class="btn">Explore Now</a>
    </div>
  </header>

  <!-- Services Section -->
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="service-cards">
      <div class="card">
        <img src="https://media.istockphoto.com/id/1526986072/photo/airplane-flying-over-tropical-sea-at-sunset.jpg?s=612x612&w=0&k=20&c=Ccvg3BqlqsWTT0Mt0CvHlbwCuRjPAIWaCLMKSl3PCks=" alt="Flight Booking">
        <h3>Flight Booking</h3>
        <p>We help you find the best deals on flights.</p>
      </div>
      <div class="card">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRi-Ef_Hg_fg5N3Pg-I3QOC32tWDBw0rc_8Ew&s" alt="Hotel Booking">
        <h3>Hotel Booking</h3>
        <p>Stay at the best hotels with our exclusive deals.</p>
      </div>
      <div class="card">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRg7MofqundYbBLMVVomhZ-LREwWL_JyYNDBg&s" alt="Custom Tours">
        <h3>Custom Tours</h3>
        <p>Personalized tours to fit your travel style.</p>
      </div>
    </div>
  </section>

  <!-- Featured Destination Section -->
  <section class="featured">
    <div class="featured-content">
      <h2>Featured Destination: Bali, Indonesia</h2>
      <p>Explore the beautiful beaches, rich culture, and vibrant nightlife of Bali. Book your dream vacation today!</p><br>
      <a href="#" class="btn">Book Now</a>
    </div>
    <div class="carousel">
    <img class="carousel-img" src="https://wallpapers.com/images/featured/bali-qhidusvhukn25lb1.jpg" alt="Bali, Indonesia">
    <img class="carousel-img" src="https://wallpapers.com/images/high/nusa-penida-beach-bali-asia-hdddql2l8dirjy1h.webp" alt="Bali, Indonesia">
    <img class="carousel-img" src="https://wallpapers.com/images/high/pulau-lan-tenga-bali-indonesia-965hrru36498v5sw.webp" alt="Bali, Indonesia">
  </div>
  </section>

  <!-- Contact Section -->
  <section class="contact">
    <h2>Contact Us</h2>
    <p>Ready to book your trip? Get in touch with us today!</p>
    <form class="contact-form">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <p>&copy; 2025 ExploreTheWorld. All rights reserved.</p>
    <i class="ri-instagram-line"></i>
    <i class="ri-facebook-circle-fill"></i>
    <i class="ri-twitter-x-line"></i>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded', function() {
      let currentIndex = 0;
      const images = document.querySelectorAll('.carousel-img');
      images[currentIndex].classList.add('active');

      setInterval(() => {
        images[currentIndex].classList.remove('active');
        currentIndex = (currentIndex + 1) % images.length;
        images[currentIndex].classList.add('active');
      }, 3000); // Change image every 3 seconds
    });
  </script>


</body>
</html>





* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    color: #333;
  }
  
  .hero {
    background-image: url('https://wallpapers.com/images/hd/travel-laptop-0m6r2w9ywrwtb81n.jpg');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    color: white;
    text-align: center;
  }
  
  .navbar {
    display: flex;
    justify-content: space-between;
    padding: 20px;
  }
  
  .logo {
    font-size: 28px;
    transition: transform 0.2s ease-in-out;
    transform: scale(1.05)
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    
  }
  
  .nav-links li {
    margin: 0 16px;
  }
  
  .nav-links a {
    color: rgb(254, 251, 251);
    text-decoration: none;
  }
  .nav-links:hover {
    transition: transform 0.3s ease-in-out;
    transform: scale(1.05)
  }  
  .hero-content {
    margin-top: 200px;
  }
  
  .hero-content h2 {
    font-size: 50px;    
  }
  
  .hero-content p {
    font-size: 18px;
    margin: 20px 0;
  }
  
  .btn {
    background-color: #ff7f50;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s;
  }
  
  .btn:hover {
    background-color: #ff4500;
  }
  
  .services {
    padding: 50px;
    text-align: center;
    background-color: #fcfdfd;
  }
  
  .services h2 {
    font-size: 36px;
    margin-bottom: 20px;
  }
  
  .service-cards {
    display: flex;
    justify-content: space-around;
    margin-top: 20px;
  }
  
  .card {
    background-color: rgb(25, 255, 224);
    padding: 20px;
    border-radius: 8px;
    width: 30%;
    box-shadow: 0 6px 9px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease-in-out;
  }

  .card:hover{
    transform: scale(1.05)
  }
  
  .card img {
    width: 100%;
    border-radius: 8px;
    /* transition: transform 0.2s ease-in-out; */
     
  }

  /* .card img:hover {
    transform: scale(1.08);
  } */
  
  .card h3 {
    margin: 10px 0;
  }
  
  .featured {
    display: flex;
    align-items: center;
    padding: 50px;
    /* transition: transform 0.5s ease-in-out; */
    background-color: #15fadf;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .featured-content {
    flex: 1;
  }
  
  .carousel {
    position: relative;
    width: 40%;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .carousel-img {
    width: 100%;
    display: none;
    transition: transform 0.3s ease-in-out;
  }
  
  .carousel-img.active {
    display: block;
  }
   


   .contact {
    padding: 50px;
    background-color: #9cf7ec;
    text-align: center;
  }
  
  .contact-form {
    display: flex;
    flex-direction: column;
    max-width: 500px;
    margin: 0 auto;
  }
  
  .contact-form input, 
  .contact-form textarea {
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #958f8f;
    border-radius: 5px;
  }
  
  .footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: white;
  }
