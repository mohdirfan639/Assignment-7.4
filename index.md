Assignment 7.4 — Modern Landing Page Header
1. Create the project files
Create a folder named Assignment-7.4 with these two files:

index.html

style.css

2. HTML code — index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header Section -->
    <header class="header">
        <nav class="navbar">
            <a href="#" class="logo">Nova<span>.</span></a>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

            <a href="#contact" class="nav-btn">Get Started</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <main>
        <section class="hero" id="home">

            <div class="hero-content">
                <p class="tagline">WELCOME TO NOVA</p>

                <h1>Build Your Future With
                    <span>Modern Technology.</span>
                </h1>

                <p class="description">
                    Discover innovative solutions that help you work
                    smarter, grow faster, and achieve your goals.
                    Start your journey with us today.
                </p>

                <div class="hero-buttons">
                    <a href="#contact" class="primary-btn">
                        Get Started
                    </a>

                    <a href="#features" class="secondary-btn">
                        Learn More →
                    </a>
                </div>

                <div class="hero-info">
                    <span>✓ Easy to use</span>
                    <span>✓ Modern design</span>
                </div>
            </div>

            <!-- Hero Illustration -->
            <div class="hero-image">
                <div class="image-card">
                    <div class="card-top">
                        <span class="dot purple"></span>
                        <span class="dot blue"></span>
                        <span class="dot pink"></span>
                    </div>

                    <div class="illustration">
                        <div class="circle"></div>

                        <div class="chart">
                            <div class="chart-bar bar-one"></div>
                            <div class="chart-bar bar-two"></div>
                            <div class="chart-bar bar-three"></div>
                            <div class="chart-bar bar-four"></div>
                            <div class="chart-bar bar-five"></div>
                        </div>

                        <div class="floating-card">
                            <span class="check-icon">✓</span>
                            <div>
                                <strong>Great Progress!</strong>
                                <p>Your goals are on track.</p>
                            </div>
                        </div>
                    </div>

                    <h3>Turn Ideas Into Reality</h3>
                    <p>Plan, create, and grow with confidence.</p>
                </div>
            </div>

        </section>

        <!-- Features Section -->
        <section class="features" id="features">
            <h2>Everything You Need to Grow</h2>
            <p>
                Simple tools, beautiful design, and powerful possibilities.
            </p>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer" id="contact">
        <p>© 2026 Nova. All rights reserved.</p>
        <a href="#home">Back to top ↑</a>
    </footer>

</body>
</html>
3. CSS code — style.css

css

/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: #202044;
    background-color: #ffffff;
    line-height: 1.6;
}

/* Header */
.header {
    width: 100%;
    background-color: #ffffff;
    box-shadow: 0 2px 15px rgba(0, 0, 0, 0.05);
    position: sticky;
    top: 0;
    z-index: 100;
}

.navbar {
    max-width: 1200px;
    min-height: 80px;
    margin: auto;
    padding: 15px 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 25px;
}

.logo {
    color: #25234d;
    font-size: 30px;
    font-weight: bold;
    text-decoration: none;
}

.logo span {
    color: #7357f5;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 32px;
    list-style: none;
}

.nav-links a {
    color: #55556b;
    text-decoration: none;
    font-size: 15px;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: #7357f5;
}

.nav-btn,
.primary-btn {
    display: inline-block;
    padding: 12px 24px;
    color: #ffffff;
    background-color: #7357f5;
    border-radius: 8px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s ease,
                transform 0.3s ease;
}

.nav-btn:hover,
.primary-btn:hover {
    background-color: #5940d4;
    transform: translateY(-2px);
}

/* Hero Section */
.hero {
    max-width: 1200px;
    min-height: 620px;
    margin: auto;
    padding: 80px 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 60px;
}

.hero-content {
    flex: 1;
    max-width: 560px;
}

.tagline {
    color: #7357f5;
    font-size: 14px;
    font-weight: bold;
    letter-spacing: 2px;
    margin-bottom: 20px;
}

.hero h1 {
    font-size: clamp(36px, 4vw, 54px);
    line-height: 1.2;
    margin-bottom: 24px;
    color: #202044;
}

.hero h1 span {
    color: #7357f5;
}

.description {
    color: #66667a;
    font-size: 17px;
    margin-bottom: 30px;
    max-width: 500px;
}

.hero-buttons {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.secondary-btn {
    color: #25234d;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}

.secondary-btn:hover {
    color: #7357f5;
}

.hero-info {
    display: flex;
    flex-wrap: wrap;
    gap: 22px;
    margin-top: 28px;
    color: #66667a;
    font-size: 14px;
}

/* Illustration */
.hero-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    min-width: 0;
}

.image-card {
    width: 100%;
    max-width: 450px;
    padding: 22px;
    background: linear-gradient(135deg, #f2efff, #e9f3ff);
    border-radius: 24px;
    box-shadow: 0 20px 50px rgba(67, 52, 150, 0.12);
}

.card-top {
    display: flex;
    gap: 7px;
    margin-bottom: 20px;
}

.dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
}

.purple {
    background: #7357f5;
}

.blue {
    background: #48a7ff;
}

.pink {
    background: #ff8fb3;
}

.illustration {
    position: relative;
    height: 260px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    border-radius: 16px;
    background-color: rgba(255, 255, 255, 0.65);
}

.circle {
    position: absolute;
    width: 190px;
    height: 190px;
    background: linear-gradient(135deg, #a99aff, #7357f5);
    border-radius: 50%;
    opacity: 0.8;
}

.chart {
    position: relative;
    z-index: 1;
    height: 145px;
    width: 210px;
    display: flex;
    align-items: flex-end;
    justify-content: center;
    gap: 12px;
}

.chart-bar {
    width: 28px;
    border-radius: 8px 8px 0 0;
    background: #ffffff;
    box-shadow: 0 4px 15px rgba(50, 40, 120, 0.12);
}

.bar-one {
    height: 45%;
}

.bar-two {
    height: 70%;
}

.bar-three {
    height: 55%;
}

.bar-four {
    height: 100%;
}

.bar-five {
    height: 80%;
}

.floating-card {
    position: absolute;
    z-index: 2;
    right: 10px;
    bottom: 15px;
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 12px;
    background: #ffffff;
    border-radius: 12px;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
}

.check-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: #e5f9ee;
    color: #20a464;
    font-weight: bold;
}

.floating-card strong {
    display: block;
    font-size: 12px;
}

.floating-card p {
    font-size: 10px;
    color: #77778a;
}

.image-card h3 {
    margin-top: 20px;
    font-size: 20px;
}

.image-card > p {
    color: #66667a;
    font-size: 14px;
}

/* Features */
.features {
    padding: 65px 25px;
    text-align: center;
    background-color: #f8f7ff;
}

.features h2 {
    font-size: 30px;
    margin-bottom: 12px;
}

.features p {
    color: #66667a;
}

/* Footer */
.footer {
    padding: 25px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 15px;
    background-color: #202044;
    color: #ffffff;
    font-size: 14px;
}

.footer a {
    color: #c5baff;
    text-decoration: none;
}

.footer a:hover {
    color: #ffffff;
}

/* Tablet */
@media (max-width: 900px) {
    .navbar {
        gap: 15px;
        padding: 15px 20px;
    }

    .nav-links {
        gap: 16px;
    }

    .hero {
        gap: 30px;
        padding: 60px 25px;
    }

    .hero h1 {
        font-size: 38px;
    }

    .image-card {
        padding: 16px;
    }
}

/* Mobile */
@media (max-width: 650px) {
    .navbar {
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .nav-links {
        order: 3;
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
        gap: 12px 22px;
        padding-top: 8px;
    }

    .nav-btn {
        padding: 10px 14px;
        font-size: 13px;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 50px 20px;
        gap: 40px;
    }

    .hero-content {
        max-width: 100%;
    }

    .hero h1 {
        font-size: 36px;
    }

    .description {
        font-size: 16px;
        margin-left: auto;
        margin-right: auto;
    }

    .hero-buttons,
    .hero-info {
        justify-content: center;
    }

    .hero-image {
        width: 100%;
    }

    .image-card {
        max-width: 450px;
        text-align: left;
    }

    .features h2 {
        font-size: 25px;
    }

    .footer {
        flex-direction: column;
        text-align: center;
    }
}

/* Small mobile screens */
@media (max-width: 380px) {
    .logo {
        font-size: 25px;
    }

    .nav-links {
        gap: 10px 15px;
    }

    .hero h1 {
        font-size: 30px;
    }

    .hero-buttons {
        flex-direction: column;
    }

    .floating-card {
        right: 5px;
        padding: 8px;
    }
}
4. Expected design
MetricFlow – Clean & Modern SaaS Hero Section UI by Shifat Ahmed on Dribbble
The code creates a clean, modern landing page with a purple accent color and a custom CSS illustration, so you don't need to download a separate image.

5. How this assignment meets the requirements
Assignment requirement

Implementation

Logo and navigation

.logo and .nav-links

Header CTA button

.nav-btn

Hero heading and paragraph

.hero-content

Hero button

.primary-btn

Illustration

.hero-image and .illustration

Side-by-side layout

display: flex on .hero

Proper alignment

align-items: center and justify-content: space-between

Footer or sticky section

Sticky .header and .footer

Responsive design

Three @media breakpoints

6. How to run the project
Save the HTML code in index.html.

Save the CSS code in style.css in the same folder.

Open index.html in your browser.

Resize the browser window to check the desktop, tablet, and mobile layouts.

Submission tip: Submit both files together. The important CSS concepts demonstrated are Flexbox, positioning, hover effects, transitions, spacing, and responsive media queries.


