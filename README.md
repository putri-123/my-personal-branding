<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Personal Branding</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f0f8ff; /* Sky Blue background */
            color: #333;
        }

        header {
            font-family: 'Dancing Script', cursive; /* Apply the new font here */
            background-color: #87ceeb; /* Sky Blue header */
            color: white;
            padding: 60px 20px;
            text-align: center;
            font-size: 3em; /* Increase font size for more impact */
            letter-spacing: 2px;
            border-bottom: 5px solid #4682b4; /* Darker Blue Border */
            animation: fadeIn 2s ease-in-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            padding: 20px;
            background-color: #4682b4; /* Darker Blue for nav */
            border-bottom: 5px solid #5f9ea0; /* Teal Border */
            animation: slideIn 1.5s ease-in-out;
        }

        @keyframes slideIn {
            from {
                transform: translateY(-100%);
            }
            to {
                transform: translateY(0);
            }
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1.2em;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #b0e0e6; /* Light Blue Hover */
            text-shadow: 0 0 5px #fff;
        }

        section {
            padding: 60px 20px;
            max-width: 1200px;
            margin: auto;
            background-color: white; /* White background for sections */
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            animation: zoomIn 1s ease-in-out;
        }

        @keyframes zoomIn {
            from {
                transform: scale(0.8);
                opacity: 0;
            }
            to {
                transform: scale(1);
                opacity: 1;
            }
        }

        .about {
            text-align: center;
        }

        .about img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 5px solid #4682b4; /* Blue border around image */
            margin-bottom: 20px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-20px);
            }
            60% {
                transform: translateY(-10px);
            }
        }

        .projects, .certificates, .skills, .lifestyle, .contact {
            background-color: #f0f8ff; /* Sky Blue background */
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);
            margin-bottom: 40px;
            animation: fadeInUp 1s ease-in-out;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h2 {
            text-align: center;
            color: #4682b4; /* Darker Blue text */
            margin-bottom: 20px;
            font-size: 2em;
        }

        .projects p, .contact p {
            color: #333;
        }

        .certificates img {
            max-width: 100%;
            height: auto;
            margin: 10px 0;
            border: 3px solid #4682b4; /* Blue border around certificates */
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: fadeIn 1.5s ease-in-out;
        }

        .skills ul {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            list-style: none;
            padding: 0;
        }

        .skills ul li {
            background-color: #4682b4; /* Sky Blue skill boxes */
            color: white;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            font-weight: bold;
            animation: fadeInLeft 1s ease-in-out;
        }

        @keyframes fadeInLeft {
            from {
                opacity: 0;
                transform: translateX(-20px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .skills ul li:hover {
            background-color: #5f9ea0; /* Teal hover effect */
        }

        .lifestyle p {
            color: #333;
            line-height: 1.8;
            font-size: 1.1em;
        }

        .contact a {
            color: #4682b4; /* Darker Blue for links */
            text-decoration: none;
            font-weight: bold;
        }

        .contact a:hover {
            text-decoration: underline;
        }

        footer {
            background-color: #87ceeb; /* Sky Blue footer */
            color: white;
            text-align: center;
            padding: 20px;
            border-top: 5px solid #4682b4; /* Darker Blue border */
            font-size: 0.9em;
            animation: fadeInUp 1s ease-in-out;
        }

        footer p {
            margin: 0;
        }

        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }

            nav ul li {
                margin: 10px 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Personal Branding Website</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#about">About Me</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#certificates">Certificates</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#lifestyle">Lifestyle & Experience</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="about" class="about">
        <h2>About Me</h2>
        <img src="profilku.jpg" alt="profilku.jpg">
        <p>Hello! I'm Putri Wulan Nurdiana, a passionate IT student. I love solving problems, learning new technologies, and creating projects that make a difference. Welcome to my personal branding website!</p>
    </section>

    <section id="projects" class="projects">
        <h2>My Projects</h2>
        <p>Project 1: My first project was learning to code</p>
        <p>Project 2: Second, I have successfully completed the large task of creating an application using the Python programming language</p>
        <p>Project 3: Third, I have just worked on a database project as a final semester assignment</p>
    </section>

    <section id="certificates" class="certificates">
        <h2>Certificates</h2>
        <img src="sertif2.jpg" alt="sertif2.jpg">
        <img src="profilpersonal.jpg" alt="profilpersonal.jpg">
    </section>

    <section id="skills" class="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML</li>
            <li>Python</li>
        </ul>
    </section>

    <section id="lifestyle" class="lifestyle">
        <h2>Lifestyle & Experience</h2>
        <p>I enjoy hiking, reading books on technology and philosophy, and participating in hackathons. In my free time, I also explore new coding challenges to improve my skills.</p>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <p>If you'd like to get in touch, feel free to reach out via email or contact me on WhatsApp number:</p>
        <p>Email: <a href="mailto:putrinurdiana28@gmail.com">putrinurdiana28@gmail.com</a></p>
        <p>Phone: <a href="phoneto:085755466505">085755466505</a></p>
    </section>

    <footer>
       
</body>
</html>
