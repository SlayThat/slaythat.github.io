# slaythat.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Polyniger Sandbox</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(45deg, #83a4d4, #b6fbff);
            color: #333;
        }

        header {
            background-color: rgba(255, 255, 255, 0.9);
            padding: 2rem;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav {
            background-color: rgba(255, 255, 255, 0.85);
            padding: 1rem;
            text-align: center;
        }

        nav a {
            margin: 0 1.5rem;
            text-decoration: none;
            color: #2c3e50;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #3498db;
        }

        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .sandbox-info {
            background: rgba(255, 255, 255, 0.9);
            padding: 2rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .projects-grid, .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .project-card, .gallery-item {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border: 2px solid #fff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .project-card:hover, .gallery-item:hover {
            transform: translateY(-5px);
        }

        footer {
            background-color: rgba(0, 0, 0, 0.8);
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 3rem;
        }

        .button {
            display: inline-block;
            padding: 0.8rem 1.5rem;
            background: #3498db;
            color: white;
            border-radius: 5px;
            text-decoration: none;
            margin-top: 1rem;
            transition: background 0.3s;
        }

        .button:hover {
            background: #2980b9;
        }

        .flag-caption {
            text-align: center;
            padding: 0.5rem;
            background: rgba(255,255,255,0.9);
            margin-top: 0.5rem;
        }

        /* Tropical OOPS Overlay */
        .oops-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.95);
            z-index: 9999;
            display: none;
            justify-content: center;
            align-items: center;
            font-size: 8rem;
            font-weight: bold;
            color: #e74c3c;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
            cursor: pointer;
            user-select: none;
            animation: tropicalOops 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
        }

        @keyframes tropicalOops {
            0% { opacity: 0; transform: rotate(-5deg) scale(0.5); }
            60% { opacity: 1; transform: rotate(2deg) scale(1.1); }
            100% { transform: rotate(0) scale(1); }
        }

        @media (max-width: 768px) {
            nav {
                display: flex;
                flex-direction: column;
                gap: 1rem;
            }
            .oops-overlay {
                font-size: 4rem;
                padding: 1rem;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>🌴 Polyniger Sandbox</h1>
        <p>Where Creativity Meets the Digital Shore</p>
    </header>

    <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">
        <section class="sandbox-info" id="about">
            <h2>Welcome to Polyniger Sandbox</h2>
            <p>A digital playground for innovative experiments, creative coding, and technological exploration. Dive into our sandbox where ideas come to life!</p>
            <a href="#projects" class="button">Explore Projects</a>
        </section>

        <section id="projects">
            <div class="sandbox-info">
                <h2>Featured Projects</h2>
                <div class="projects-grid">
                    <div class="project-card">
                        <h3>3D Terrain Generator</h3>
                        <p>Explore procedurally generated landscapes using WebGL</p>
                        <a href="#" class="button">Try Demo</a>
                    </div>
                    <div class="project-card">
                        <h3>AI Art Studio</h3>
                        <p>Create unique artworks with machine learning models</p>
                        <a href="#" class="button">Start Creating</a>
                    </div>
                    <div class="project-card">
                        <h3>Physics Simulator</h3>
                        <p>Interactive particle physics simulation playground</p>
                        <a href="#" class="button">Launch Sim</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Gallery Section -->
        <section id="gallery">
            <div class="sandbox-info">
                <h2>International Gallery</h2>
                <p>Explore cultural inspirations from around the world</p>
                <div class="gallery-grid">
                    <div class="gallery-item">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Flag_of_Bulgaria.svg/1280px-Flag_of_Bulgaria.svg.png" 
                             alt="Bulgarian Flag">
                        <div class="flag-caption">
                            <h3>Bulgarian Flag</h3>
                            <p>Трикольорът на гордостта (The Tricolor of Pride)</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="sandbox-info">
                <h2>Contact Us</h2>
                <p>Have questions or want to collaborate? Get in touch!</p>
                <p>Email: contact@polyniger-sandbox.com</p>
            </div>
        </section>
    </div>

    <!-- OOPS Overlay -->
    <div class="oops-overlay" onclick="this.style.display = 'none'">OOPS!</div>

    <footer>
        <p>© 2023 Polyniger Sandbox. All rights reserved.</p>
        <div style="margin-top: 1rem;">
            <a href="#" style="color: #3498db; margin: 0 0.5rem;">Twitter</a>
            <a href="#" style="color: #3498db; margin: 0 0.5rem;">GitHub</a>
            <a href="#" style="color: #3498db; margin: 0 0.5rem;">Instagram</a>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const buttons = document.querySelectorAll('.project-card .button');
            
            buttons.forEach(button => {
                button.addEventListener('click', function(e) {
                    e.preventDefault();
                    const overlay = document.querySelector('.oops-overlay');
                    overlay.style.display = 'flex';
                    
                    // Reset animation
                    void overlay.offsetWidth;
                    overlay.style.animation = 'none';
                    setTimeout(() => {
                        overlay.style.animation = 'tropicalOops 0.6s cubic-bezier(0.34, 1.56, 0.64, 1)';
                    }, 10);
                });
            });
        });
    </script>
</body>
</html>
