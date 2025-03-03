<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NEHA - Luxury Bags</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fff;
            color: #333;
        }
        header {
            background-color: #ff0000;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav {
            margin: 10px 0;
            text-align: center;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: white;
        }
        .banner {
            background-image: url('banner.jpg');
            background-size: cover;
            color: white;
            padding: 50px;
            text-align: center;
        }
        .content {
            margin: 20px;
        }
        .content h2 {
            color: #ff0000;
        }
        .testimonial, .faq {
            background-color: #f9f9f9;
            black: 20px;
            margin: 20px 0;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        .gallery img {
            width: 100%;
            max-width: 200px;
            height: auto;
            border: 1px solid #ccc;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
        }
        form {
            display: flex;
            flex-direction: column;
            max-width: 400px;
            margin: 0 auto;
        }
        label, input, textarea {
            margin: 10px 0;
            padding: 10px;
            font-size: 16px;
        }
        input[type="submit"] {
            background-color: #ff0000;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            console.log('Welcome to NEHA!');
        });
    </script>
</head>
<body>
    <header>
        <h1>NEHA</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About Us</a>
            <a href="#services">Services</a>
            <a href="#testimonials">Testimonials</a>
            <a href="#gallery">Gallery</a>
            <a href="#faq">FAQ</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <section class="banner" id="home">
        <h2>Your comfort, Our Priority</h2>
        <p>Providing luxury for over 15 years.</p>
        <p>Contact us: 9205490534 | adityaa.ch2010@gmail.com</p>
    </section>
    <section class="content" id="about">
        <h2>About Us</h2>
        <p>NEHA  is a luxury bag brand which offer expensive bags which is available at NEHA only they are mainly 5 in the world which make it rare. We are providing this lifestyle over 15 years in which we have provided bags tomore than 1500 customers it include Ambani's and Adani's also. We import the things from all over the world to make each bag that make it expensive.</p>
        <h3>Our Mission</h3>
        <p>To ensure the lifestyle of our clients through comprehensive bags</p>
        <h3>Owner's Message</h3>
        <p>Make your personality good by shoping with NEHA</p>
    </section>
    <section class="content" id="services">
        <h2>Our PRODUCTS</h2>
        <p>We provide a wide range of exclusive bags and rare bags which is mostly made with rare metals from all over the world with heart.</p>
        <h3>HIGH QUALITY</h3>
        <p>We provide high quality bags which is very relaible because of the expensive materials used in it with our love and care</p>
    </section>
    <section class="content testimonial" id="testimonials">
        <h2>Testimonials</h2>
        <p>"NEHA bags have good quality Highly recommend!" - Aditya</p>
        <p>"It has a good space" - Rohan</p>
        <p>" We like the rare things and NEHA offers rare bags" - Nita ambani</p>
    </section>
    <section class="content gallery" id="gallery">
        <h2>Gallery</h2>
                <img src="firetruck.jpg" alt="American Bag with 100 Diamond">
        <img src="fire_extinguisher.jpg" alt="European Bag with 56 Rare stones">
        <img src="no.jpg" alt="Indian Bag with 22 carat gold of 20gram">
        <img src="no.jpg" alt="Singapore Bag made with platinum">
    </section>
    <section class="content faq" id="faq">
        <h2>FAQ</h2>
        <h3>What is different in your bags?</h3>
        <p>We offer good and fancy bags which is only available at NEHA</p>
        <h3>How can we contact you?</h3>
        <p>You can contact us via phone at 9205490534 or email at adityaa.ch2010@gmail.com.</p>
        <h3>Is the bags customisable?</h3>
        <p> We mostly try to customize it as the customber need and to fullfil all the wants of customes to make our customer experiance good but sometime we reject the demand of customize if it not fit in our standard or something not possible or realistic.</p>
    </section>
    <section class="content" id="contact">
        <h2>Contact Us</h2>
        <p>Phone: 9319076712</p>
        <p>Email: sahneha678@gmail.com</p>
        <form action="https://formspree.io/f/adityaa.ch2010@gmail.com" method="POST">
            <?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    // Collect form data
    $name = $_POST['name'];
    $email = $_POST['email'];
    $phone = $_POST['phone'];
    
    // Email address where you want to receive emails
    $to = "adityaa.ch2010@gmail.com"; // Replace with your email address
    
    // Subject of the email
    $subject = "New Contact Form Submission";
    
    // Compose the email content
    $message = "Name: $name\n";
    $message .= "Email: $email\n";
    $message .= "Phone Number: $phone\n";
    
    // Set headers
    $headers = "From: $email\r\n";
    $headers .= "Reply-To: $email\r\n";
    
    // Attempt to send email
    if (mail($to, $subject, $message, $headers)) {
        echo "Thank you for your message. We will contact you shortly.";
    } else {
        echo "Oops! Something went wrong and we couldn't send your message.";
    }
} else {
    echo "There was a problem with your submission, please try again.";
}
?>
Send feedback on sahneha678@gmail.com
        </form>
    </section>
    <footer>
        <p>&copy; 2025 NEHA. All rights reserved.</p>
    </footer>
</body>
</html>
