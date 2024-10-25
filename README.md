# imangembali.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hotel L</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <img src="images/logo.png" alt="Hotel Logo" class="logo">
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="rooms.html">Rooms</a></li>
                <li><a href="dining.html">Dining</a></li>
                <li><a href="amenities.html">Amenities</a></li>
                <li><a href="bookings.html">Bookings</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-text">
            <h1>Welcome to Hotel L, Your Oasis of Comfort</h1>
            <a href="bookings.html" class="cta-button">Book Now</a>
        </div>
    </section>

    <section class="features">
        <div class="feature-box">
            <h2>Luxury Rooms</h2>
            <p>Experience ultimate comfort and elegance in our luxury rooms.</p>
        </div>
        <div class="feature-box">
            <h2>Fine Dining</h2>
            <p>Indulge in gourmet dining at our world-class restaurant.</p>
        </div>
        <div class="feature-box">
            <h2>Exceptional Service</h2>
            <p>Our staff is dedicated to making your stay unforgettable.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Hotel L. All Rights Reserved.</p>
    </footer>

    <script src="js/main.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    color: #333;
    background-color: #f0f8ff;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #005b96;
}

.logo {
    width: 100px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

.hero {
    background: url('images/hotel-hero.jpg') no-repeat center center/cover;
    height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero-text h1 {
    font-size: 48px;
    margin-bottom: 20px;
    font-family: 'Georgia', cursive;
}

.cta-button {
    padding: 10px 20px;
    background-color: #0074d9;
    color: white;
    text-decoration: none;
    border-radius: 5px;
}

.cta-button:hover {
    background-color: #005b96;
}

.features {
    display: flex;
    justify-content: space-around;
    padding: 50px 0;
    background-color: #fff;
}

.feature-box {
    text-align: center;
    padding: 20px;
    background-color: #e0f7fa;
    border-radius: 10px;
    width: 30%;
}

.feature-box h2 {
    margin-bottom: 15px;
    color: #005b96;
}

footer {
    background-color: #005b96;
    color: white;
    text-align: center;
    padding: 20px 0;
    margin-top: 40px;
}
document.addEventListener('DOMContentLoaded', function () {
    console.log('Hotel L website loaded');
});
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rooms | Hotel L</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <img src="images/logo.png" alt="Hotel Logo" class="logo">
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="rooms.html">Rooms</a></li>
                <li><a href="dining.html">Dining</a></li>
                <li><a href="amenities.html">Amenities</a></li>
                <li><a href="bookings.html">Bookings</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="rooms-overview">
        <h1>Our Rooms</h1>
        <div class="room-grid">
            <div class="room-box">
                <img src="images/room1.jpg" alt="Luxury Room">
                <h2>Luxury Room</h2>
                <p>Price: $200 per night</p>
                <a href="bookings.html" class="cta-button">Book Now</a>
            </div>
            <!-- Add more room boxes here -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Hotel L. All Rights Reserved.</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bookings | Hotel L</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <img src="images/logo.png" alt="Hotel Logo" class="logo">
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="rooms.html">Rooms</a></li>
                <li><a href="dining.html">Dining</a></li>
                <li><a href="amenities.html">Amenities</a></li>
                <li><a href="bookings.html">Bookings</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="booking-form">
        <h1>Book Your Stay</h1>
        <form>
            <label for="room-type">Room Type:</label>
            <select id="room-type" name="room-type">
                <option value="luxury-room">Luxury Room</option>
                <option value="standard-room">Standard Room</option>
            </select>

            <label for="check-in">Check-in Date:</label>
            <input type="date" id="check-in" name="check-in">

            <label for="check-out">Check-out Date:</label>
            <input type="date" id="check-out" name="check-out">

            <label for="guests">Guests:</label>
            <input type="number" id="guests" name="guests" min="1" max="5">

            <button type="submit" class="cta-button">Reserve Now</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Hotel L. All Rights Reserved.</p>
    </footer>
</body>
</html>
