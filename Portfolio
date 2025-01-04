<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Portfolio</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f7fc;
            color: #333;
            line-height: 1.6;
            transition: all 0.3s ease;
        }

        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: #003366;
            color: white;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        nav {
            display: flex;
            justify-content: center;
            padding: 1em 0;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 2em;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-size: 1.2em;
            font-weight: 500;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        .nav-links a:hover {
            color: #00aaff;
            transform: scale(1.1);
        }

        .section {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            font-size: 2.5em;
            color: white;
            animation: fadeIn 1.5s ease-in-out;
            transition: background-color 0.5s ease;
        }

        #home {
            background: linear-gradient(135deg, #003366, #0055a5);
        }

        #about {
            background: linear-gradient(135deg, #0055a5, #0077cc);
        }

        #portfolio {
            background: linear-gradient(135deg, #0077cc, #3399ff);
        }

        #contact {
            background: linear-gradient(135deg, #3399ff, #66ccff);
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        .info-section {
            max-width: 900px;
            margin: 0 auto;
            padding: 3em;
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .info-section h2 {
            margin-bottom: 1em;
            font-size: 2.5em;
            color: #003366;
        }

        .info-section p {
            font-size: 1.2em;
            line-height: 1.6;
            color: #555;
        }

        .skills {
            display: flex;
            justify-content: space-around;
            margin-top: 3em;
        }

        .skill {
            text-align: center;
            width: 150px;
        }

        .skill i {
            font-size: 3.5em;
            color: #0077cc;
            transition: transform 0.3s ease, color 0.3s ease;
        }

        .skill h4 {
            margin-top: 10px;
            font-size: 1.2em;
        }

        .skill:hover i {
            transform: rotate(20deg) scale(1.2);
            color: #00aaff;
        }

        .languages {
            margin-top: 2em;
        }

        .languages h3 {
            margin-bottom: 1.5em;
            color: #003366;
            font-size: 2em;
            font-weight: 700;
            text-transform: uppercase;
        }

        .bar {
            width: 100%;
            height: 20px;
            background-color: #e0f7fa;
            border-radius: 12px;
            margin-bottom: 2em;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            position: relative;
        }

        .progress {
            height: 100%;
            border-radius: 12px;
            text-align: center;
            color: black; /* Change text color for better contrast */
            line-height: 20px;
            font-weight: bold;
            width: 0%;
            animation: progressAnim 2s forwards;
        }

        @keyframes progressAnim {
            0% {
                width: 0%;
            }
            100% {
                width: 100%;
            }
        }

        #html {
            background-color: #2196f3; /* Blue */
        }

        #css {
            background-color: #4caf50; /* Green */
        }

        #js {
            background-color: #ff9800; /* Orange */
        }

        #react {
            background-color: #9c27b0; /* Purple */
        }

        .bar:hover .progress {
            transition: width 1s ease-in-out;
        }

        .languages .bar {
            animation: growBar 3s ease-in-out infinite;
        }

        @keyframes growBar {
            0% {
                width: 0%;
            }
            50% {
                width: 100%;
            }
            100% {
                width: 0%;
            }
        }

        /* Contact Form */
        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 1.5em;
            margin-top: 2em;
            text-align: left;
        }

        .contact-form input, .contact-form textarea {
            padding: 1em;
            font-size: 1em;
            border: 2px solid #0077cc;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            outline: none;
            border-color: #00aaff;
            box-shadow: 0 0 8px rgba(0, 170, 255, 0.5);
        }

        .contact-form button {
            background-color: #0077cc;
            color: white;
            font-size: 1.2em;
            padding: 1em;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .contact-form button:hover {
            background-color: #00aaff;
            transform: scale(1.05);
        }

        /* Animation for scrolling */
        .smooth-scroll {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="smooth-scroll">

    <header>
        <nav>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="section">
        <div>
            <h1>Welcome to My Portfolio</h1>
            <p>I'm Mays Waleed Owais, a passionate front-end developer and computer science student.</p>
        </div>
    </section>

    <!-- About Me Section -->
    <section id="about" class="section" style="background: linear-gradient(135deg, #0055a5, #0077cc);">
        <div class="info-section">
            <h2>About Me</h2>
            <p>I'm a third-year Computer Science student at Jerash University. My goal is to create innovative and user-friendly web applications. I have experience in web development technologies like HTML, CSS, JavaScript, and React.</p>
            <p>In my free time, I enjoy solving coding challenges, learning new technologies, and building fun projects like interactive coding games and educational websites.</p>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="section" style="background: linear-gradient(135deg, #0077cc, #3399ff);">
        <div class="info-section">
            <h2>My Work</h2>
            <p>Here are some of the projects I've worked on:</p>
            <div class="skills">
                <div class="skill">
                    <i class="fas fa-laptop-code"></i>
                    <h4>Web Development</h4>
                </div>
                <div class="skill">
                    <i class="fas fa-cogs"></i>
                    <h4>Programming</h4>
                </div>
                <div class="skill">
                    <i class="fas fa-gamepad"></i>
                    <h4>Interactive Games</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Languages Section -->
    <section id="languages" class="section">
        <div class="info-section languages">
            <h3>Languages I Master</h3>
            <div class="bar">
                <div class="progress" id="html" style="width: 90%;">HTML (90%)</div>
            </div>
            <div class="bar">
                <div class="progress" id="css" style="width: 80%;">CSS (80%)</div>
            </div>
            <div class="bar">
                <div class="progress" id="js" style="width: 75%;">JavaScript (75%)</div>
            </div>
            <div class="bar">
                <div class="progress" id="react" style="width: 65%;">React (65%)</div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section" style="background: linear-gradient(135deg, #3399ff, #66ccff);">
        <div class="info-section">
            <h2>Contact Me</h2>
            <p>If you'd like to get in touch or collaborate on a project, feel free to reach out!</p>
            <form class="contact-form">
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" rows="4" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>

</body>
</html>
