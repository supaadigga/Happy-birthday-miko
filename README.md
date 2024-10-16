<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Birthday ni Micko-chan</title>
    
    <!-- Bootstrap CDN -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            background-color: #1a1a1a;
            font-family: 'Poppins', sans-serif;
        }

        /* Welcome Page Styles */
        .welcome-section {
            position: relative;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column; /* Center items vertically */
            background-color: #000;
            overflow: hidden;
        }

        .welcome-image {
            width: 150px; /* Set width of the welcome image */
            border-radius: 10px; /* Optional: Add some rounding to the image */
            margin-bottom: 20px; /* Space between image and title */
        }

        .welcome-content {
            text-align: center;
            color: #fff;
        }

        .welcome-btn {
            margin-top: 20px;
            padding: 10px 30px;
            font-size: 1.2rem;
            background-color: #ff6f61;
            border: none;
            border-radius: 5px;
            color: #fff;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .welcome-btn:hover {
            background-color: #ff4940;
        }

        /* Carousel Page Styles */
        .carousel-container {
            margin: 50px auto;
            width: 95%; /* Adjust width of the carousel */
            max-width: 1200px; /* Increase the maximum width */
            border-radius: 20px;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.8);
        }

        .carousel-inner img {
            width: 100%;
            height: 600px; /* Increase height of the images */
            object-fit: cover; /* Ensures the image covers the box without distortion */
            border-radius: 20px;
            border: 20px solid #333; /* Bigger border */
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.8); /* Larger shadow */
        }

        .carousel-control-prev-icon,
        .carousel-control-next-icon {
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            width: 40px;
            height: 40px;
        }

        .carousel-caption {
            background: rgba(0, 0, 0, 0.5);
            border-radius: 10px;
            padding: 12px;
            font-size: 1.5rem;
        }

        /* Video Styles */
        .video-container {
            text-align: center;
            margin: 50px 0;
        }

        video {
            max-width: 30%;
            height: 5%;
            border-radius: 10px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.8);
        }
    </style>
</head>
<body>

<!-- Home Page -->
<div class="welcome-section" id="home">
    <img src="meko.png" alt="Welcome" class="welcome-image"> <!-- Add your welcoming image -->
    <div class="welcome-content">
        <h1>Happy Birthday Micko!</h1>
        <button class="welcome-btn" onclick="window.location.href='#carousel'">Explore My Baby</button>
        <!-- Link updated to scroll to video -->
        <button class="welcome-btn" onclick="window.location.href='#videoSection'">Watch the Video</button>
    </div>
</div>

<!-- Carousel Page -->
<div id="carousel" class="carousel slide carousel-container" data-bs-ride="carousel">
    <!-- Dots/Indicators -->
    <div class="carousel-indicators">
        <button type="button" data-bs-target="#carousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
        <button type="button" data-bs-target="#carousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
        <button type="button" data-bs-target="#carousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>

    <!-- Carousel Items -->
    <div class="carousel-inner">
        <div class="carousel-item active">
            <img src="miko 1.jpg" class="d-block w-100" alt="Slide 1">
            <div class="carousel-caption">
                My Baby
            </div>
        </div>
        <div class="carousel-item">
            <img src="miko 2.jpg" class="d-block w-100" alt="Slide 2">
            <div class="carousel-caption">
                Baby Ko 
            </div>
        </div>
        <div class="carousel-item">
            <img src="miko w.png" class="d-block w-100" alt="Slide 3">
            <div class="carousel-caption">
                So Cute!
            </div>
        </div>
    </div>

    <!-- Navigation buttons -->
    <button class="carousel-control-prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carousel" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
    </button>
</div>

<!-- Video Section -->
<div id="videoSection" class="video-container">
    <h2 style="color: #fff;">Enjoy the Video!</h2>
    <video controls autoplay muted loop style="width: 80%; height: auto;">
        <source src="videos/mikoVideo.mp4" type="video/mp4"> <!-- Update the path as needed -->
        Your browser does not support the video tag.
    </video>
</div>

<!-- Bootstrap JS and Popper.js -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
