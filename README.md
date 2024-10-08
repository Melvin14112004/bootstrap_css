# bootstrap_css

## HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doom Eternal</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Roboto+Condensed:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header-container">
        <img src="img/38.jpg" alt="Doom Eternal Header Image" class="header-image"> <!-- Huge fluid image -->
        <div class="header-content">
            <h1>Doom Eternal</h1>
            <h2>Rip and Tear</h2>
            <a href="#about" class="btn btn-danger">Learn More</a>
            <a href="#media" class="btn btn-dark">See Media</a>
        </div>
    </header>
    <section id="about" class="container text-center">
        <h2>About Doom Eternal</h2>
        <p>Doom Eternal is a relentless, pulse-pounding first-person shooter that pushes the boundaries of what a shooter can be...</p>
    </section>
    <section id="gameplay" class="container text-center">
        <h2>Gameplay</h2>
        <div class="row">
            <div class="col-md-4">
                <img src="img/rip.jpeg" class="img-fluid" alt="Gameplay Feature 1">
                <h3>Rip and Tear</h3>
                <p>Engage in brutal, fast-paced combat</p>
            </div>
            <div class="col-md-4">
                <img src="img/chain.jpg" class="img-fluid" alt="Gameplay Feature 2">
                <h3>Chainsaw</h3>
                <p>Slash it for ammo, and health</p>
            </div>
            <div class="col-md-4">
                <img src="img/dash.jpeg" class="img-fluid" alt="Gameplay Feature 3">
                <h3>Dash</h3>
                <p>To move around quickly, to slay demons</p>
            </div>
        </div>
    </section>
    <section id="media" class="text-center py-5">
        <div class="container">
            <h2>Media</h2>
            <div class="row">
                <div class="col-md-4">
                    <img src="img/1.jpg" class="img-fluid" alt="Media 1">
                </div>
                <div class="col-md-4">
                    <img src="img/2.jpg" class="img-fluid" alt="Media 2">
                </div>
                <div class="col-md-4">
                    <img src="img/3.jpeg" class="img-fluid" alt="Media 3">
                </div>
            </div>
        </div>
    </section>
    <section id="news" class="container text-center">
        <h2>Latest News</h2>
        <div class="row">
            <div class="col-md-4">
                <img src="img/4.jpg" class="img-fluid" alt="News Item 1">
                <h3>Part 2</h3>
                <p>The Slayer Chronicles continue</p>
                <a href="#" class="btn btn-outline-danger">Read More</a>
            </div>
            <div class="col-md-4">
                <img src="img/5.png" class="img-fluid" alt="News Item 2">
                <h3>New Bosses</h3>
                <p>Rip and Tear till death</p>
                <a href="#" class="btn btn-outline-danger">Read More</a>
            </div>
            <div class="col-md-4">
                <img src="img/6.jpg" class="img-fluid" alt="News Item 3">
                <h3>News Areas</h3>
                <p>New updates and expansions</p>
                <a href="#" class="btn btn-outline-danger">Read More</a>
            </div>
        </div>
    </section>
    <section id="contact" class="bg-black text-white text-center py-5"> <!-- Changed bg-dark to bg-black -->
        <div class="container">
            <h2>Contact Us</h2>
            <form class="contact-form">
                <div class="form-group">
                    <input type="text" class="form-control" placeholder="Your Name">
                </div>
                <div class="form-group">
                    <input type="email" class="form-control" placeholder="Your Email">
                </div>
                <div class="form-group">
                    <textarea class="form-control" rows="5" placeholder="Your Message"></textarea>
                </div>
                <button type="submit" class="btn btn-danger">Send Message</button>
            </form>
        </div>
    </section>
    <footer class="text-center py-3">
        <p>&copy; 2024 Doom Eternal. All Rights Reserved.</p>
    </footer>
</body>
</html>
```

## CSS

```css
body {
    font-family: 'Roboto Condensed', sans-serif;
    background-color: #000000;
    color: #FFFFFF;
    background-image: url('doom-eternal-bg.jpg');
    background-size: cover;
    background-attachment: fixed;
    margin: 0;
    padding: 0;
}

header {
    position: relative;
    height: 600px;
    overflow: hidden;
}

.header-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
}

.header-content {
    position: relative;
    padding: 200px 20px; 
    text-align: center;
}

header h1 {
    font-family: 'Bangers', cursive;
    font-size: 5rem;
    color: white; 
    margin-bottom: 20px;
    z-index: 2;
}

header h2 {
    font-size: 3rem;
    color: white;
    margin-bottom: 20px;
    z-index: 2;
}

header .btn {
    background-color: darkred;
    border: 3px solid darkred; 
    color: #FFFFFF;
    font-weight: bold;
    text-transform: uppercase;
    margin: 10px;
    z-index: 2;
}

header .btn:hover {
    background-color: white;
    color: #FFFFFF;
    text-shadow: 1px 1px 4px darkred;
}

section {
    padding: 60px 0;
    background: rgba(0, 0, 0, 0.9); 
    color: #FFFFFF;
    position: relative;
}

h2 {
    font-family: 'Bangers', cursive;
    font-size: 3rem;
    color: white;
    margin-bottom: 30px;
    text-transform: uppercase;
    text-shadow: 2px 2px 4px darkred;
    position: relative;
}

p {
    font-size: 1.2rem;
    line-height: 1.8;
    position: relative;
}

#gameplay img,
#news img {
    border: 5px solid darkred;
    transition: transform 0.3s ease;
    box-shadow: 0px 0px 15px 3px 5px darkred;
    margin-bottom: 20px;
}

#gameplay img:hover,
#news img:hover {
    transform: scale(1.05);
    filter: brightness(80%);
}

footer {
    background-color: black; 
    padding: 30px 0;
    color: white; 
    text-align: center;
    position: relative;
}

footer::before {
    content: "";
    background: url('footer-blood-drip.png') no-repeat bottom center;
    background-size: cover;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    opacity: 0.8;
    z-index: 1;
}

footer p {
    margin: 0;
    z-index: 2;
    position: relative;
}

.contact-form {
    background-color: black; 
    padding: 30px;
    border-radius: 10px;
    border: 2px solid white;
    position: relative;
}

.contact-form .form-control {
    background-color: black; 
    color: white;
    border: 1px solid white;
}

.contact-form .btn-danger {
    background-color: darkred;
    border-color: white;
    font-weight: bold;
    text-transform: uppercase;
}

.contact-form .btn-danger:hover {
    background-color: white;
    border-color: white;
}