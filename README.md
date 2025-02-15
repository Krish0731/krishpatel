<!DOCTYPE html>
<html>
<head>
    <title>Krish's Homepage</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: LightBlue;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }

        .logo {
            font-size: 100px;
            font-weight: bold;
            text-shadow: 0 0 5px rgba(255, 0, 0, 0.8);
            animation: textShadow 3s ease-in-out infinite alternate;
        }

        @keyframes textShadow {
            0% {
                text-shadow: 0 0 5px rgba(255, 0, 0, 0.8);
            }
            100% {
                text-shadow: 0 0 10px rgba(0, 0, 255, 0.8);
            }
        }

        nav {
            background-color: #444;
            text-align: center;
            padding: 10px;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav li {
            display: inline;
            margin-right: 20px;
            font-size: 28px;
        }

        nav a {
            text-decoration: none;
            color: #fff;
            font-weight: bold;
            font-family: 'Arial', sans-serif;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #ff5722;
        }

        .dropdown {
            position: relative;
            display: inline-block;
        }

        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #333;
            min-width: 160px;
            z-index: 1;
        }

        .dropdown-content a {
            padding: 10px 20px;
            display: block;
            color: #fff;
            text-decoration: none;
        }

        .dropdown:hover .dropdown-content {
            display: block;
        }

        table {
            width: 100%;
            border-collapse: collapse;
        }

        th, td {
            padding: 15px;
            text-align: left;
        }

        th {
            background: linear-gradient(to right, #D6EEEE, #D6D6EE);
            font-size: 24px;
        }

        td {
            background: linear-gradient(to right, #D1EFF5, #D1D1F5);
            font-size: 20px;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Welcome to Krish's Homepage</div>
    </header>

    <nav>
        <ul>
            <li><a href="index.html">About Me</a></li>
            <li class="dropdown">
                <a href="Resume.html">Resume</a>
                <div class="dropdown-content">
                    <a href="Resume.html">View Resume</a>
                    <a href="DownloadResume.html" target="_blank">Download Resume</a>
                </div>
            </li>
            <li><a href="Emerging_Tech_Expert.html">Virtual Reality</a></li>
            <li><a href="contact.html">Feedback</a></li>
            <li><a href="cite.html">Citation</a></li>
        </ul>
    </nav>

    <hr>
    <ul style="font-family: Arial; font-size: 20px;">
        <li><em>Name:</em> <strong>Krish Patel</strong></li>
        <li><em>Age:</em> <strong>15</strong></li>
        <li><em>Interest:</em> <strong>Watching Apple Events and Watching Tech reviews</strong></li>
        <li><em>Hobbies:</em> <strong>Watching Cricket</strong></li>
        <li><em>Career Goal:</em> <strong>Computer Scientist</strong></li>
    </ul>
    <hr>
    <h1 style="color: Red; text-align: Center; font-size: 60px; font-family: Georgia;">Table Of Projects</h1>
    <hr>
    <table border="5">
        <tr>
            <th style="font-size: 50px">Project Title</th>
            <th style="font-size: 50px">Description</th>
            <th style="font-size: 50px">Completion Due</th>
        </tr>
        <tr>
            <td style="font-size: 40px"><a href="Adventure.html">Adventure Story Website</a></td>
            <td style="font-size: 40px">A website that takes the user through a short computer science adventure story.</td>
            <td style="font-size: 40px">September 5, 2023</td>
        </tr>
        <tr>
            <td style="font-size: 40px"><a href="Emerging_Tech_Expert.html">Emerging Tech Expert Website</a></td>
            <td style="font-size: 40px">A website about Virtual Reality to educate others.</td>
            <td style="font-size: 40px">Oct 11, 2023</td>
        </tr>
    </table>
</body>
</html>
