
 import zipfile
import os

# Create the directory structure and files
directory = "/mnt/data/technology_insights"
os.makedirs(directory, exist_ok=True)

# HTML content
html_content = """
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Technology Insights</title>
    <style>
        body {
            font-family: "Times New Roman", Times, serif;
            margin: 0;
            padding: 0;
            font-size: 12px;
            line-height: 1.5;
            text-align: justify;
        }

        nav {
            background-color: #333;
            color: rgb(15, 193, 224);
            padding: 1rem;
            text-align: center;
        }

        nav a {
            color: rgb(255, 255, 255);
            margin: 0 15px;
            text-decoration: none;
        }

        nav a:hover {
            text-decoration: underline;
        }

        header, footer {
            background-color: #11c1e0;
            padding: 2rem;
            text-align: center;
        }

        section {
            padding: 2rem;
            max-width: 900px;
            margin: auto;
        }

        h1, h2, h3 {
            font-size: 14px;
            font-weight: bold;
            text-align: left;
        }

        .gallery img {
            width: 100%;
            max-width: 300px;
            margin: 10px;
        }

        .contact-form {
            display: flex;
            flex-direction: column;
        }

        .contact-form input,
        .contact-form textarea {
            margin-bottom: 1rem;
            padding: 0.5rem;
            font-size: 1rem;
        }

        .instruction-materials {
            background-color: #eef;
            padding: 1rem;
            margin: 2rem 0;
            border-left: 4px solid #33a;
        }

        figure {
            margin: 1rem 0;
            max-width: 45%;
        }

        figure img {
            width: 100%;
            height: auto;
        }

        figure figcaption {
            font-size: 12px;
            text-align: center;
            margin-top: 0.5rem;
        }
    </style>
</head>

<body>
    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
        <a href="gallery.html">Gallery</a>
        <a href="resources.html">Resources</a>
        <a href="contact.html">Contact</a>
    </nav>

    <header>
        <h1>Technology Insights</h1>
        <p>Developed by Derrick Semefa</div></p>
        <p>Presented on [Not Published]</p>
    </header>

    <section>
        <h2>Introduction</h2>
        <p>Welcome to Technology Insights, a platform dedicated to exploring the latest trends and developments in technology. Use the navigation bar to learn more.</p>
        <figure>
            <video width="100%" controls>
                <source src="media/tech-overview.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
            <figcaption>Figure 1.1: Technology Overview Video</figcaption>
        </figure>

        <p>As shown in Figure 1.1, the video provides a broad overview of current technological advancements.</p>

        <figure>
            <audio controls>
                <source src="media/tech-podcast.mp3" type="audio/mpeg">
                Your browser does not support the audio element.
            </audio>
            <figcaption>Figure 1.2: Podcast on Emerging Technologies</figcaption>
        </figure>

        <p>Listen to the podcast in Figure 1.2 for insights into emerging technologies shaping our future.</p>

        <div class="gallery">
            <h3>Gallery</h3>
            <figure>
                <img src="media/ai-robotics.jpg" alt="AI and Robotics">
                <figcaption>Figure 1.3: AI and Robotics</figcaption>
            </figure>
            <figure>
                <img src="media/quantum-computing.jpg" alt="Quantum Computing">
                <figcaption>Figure 1.4: Quantum Computing</figcaption>
            </figure>
            <figure>
                <img src="media/smart-cities.jpg" alt="Smart Cities">
                <figcaption>Figure 1.5: Smart Cities</figcaption>
            </figure>
        </div>

        <div class="instruction-materials">
            <h3>Instructional Materials</h3>
            <ul>
                <li><a href="media/tech-guide.pdf" target="_blank">Download Technology Guide PDF</a></li>
                <li><a href="media/coding-tutorial.mp4" target="_blank">Watch Coding Tutorial</a></li>
                <li><a href="media/tech-trends.html" target="_blank">Read About Tech Trends</a></li>
            </ul>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Derrick. All Rights Reserved.</p>
        <p>Follow us on 
            <a href="https://twitter.com" target="_blank">Twitter</a>, 
            <a href="https://facebook.com" target="_blank">Facebook</a>, and 
            <a href="https://instagram.com" target="_blank">Instagram</a>.
        </p>
    </footer>
</body>

</html>
"""
