<!DOCTYPE html>
<html>
  <head>
    <title>Krish's Homepage</title>    
        <style>
        header{
        background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        
        
        .logo {
            font-size: 100px;
            font-weight: bold;
        }
        
        
        nav {
            background-color: #444;
            text-align: center;
        }
        
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        
        nav li {
            display: inline;
            margin-right: 50px;
        }
        
        nav a {
            text-decoration: none;
            color: #fff;
            font-weight: bold;
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
            padding: 50px 50px;
            display: block;
            color: #fff;
            text-decoration: none;
        }
        
        .dropdown:hover .dropdown-content {
            display: block;
        }
        ul {
            font-size: 40px;
            color: Green;
            font-family: "Lucida Console", "Courier New", monospace;
}
        }

 body {
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #f0f0f0;
}
}
    table {
      width: 100%;
      border-collapse: collapse;
    }

    th,
    td {
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
       0% {
        background: linear-gradient(to right, #333, #111);
      }
      100% {
        background: linear-gradient(to right, #111, #333);
      }
    }
 nav {
      background-color: #444;
      text-align: center;
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

    </style>
    
  </head>
  <header>
        <div class="logo">Welcome to Krish's Homepage</div>
    </header>

    <nav>
        <ul>
            <li style="font-size:50px"><a href="index.html">About Me</a></li>
            <li class="dropdown" style="font-size:50px">
          <a href="Resume.html">Resume</a>
          <div class="dropdown-content">
            <a href="Resume.html">View Resume</a>
            <a href="DownloadResume.html" target="_blank">Download Resume</a>
            </li>
            <li style="font-size:50px"><a href="Emerging_Tech_Expert.html">Virtual Reality</a></li>
            <li style="font-size:50px"><a href="contact.html">Feedback</a></li>
            <li style="font-size:50px"><a href="cite.html">Citation</a></li>
        </ul>
    </nav>
  <body style="background-color: LightBlue">
    <hr>
    <ul style="font-family: Arial">       
      <li><em>Name:</em> <strong>Krish Patel</strong></li>
        <li><em>Age:</em>  <strong>15</strong></li>
        <li><em>Interest:</em> <strong> Watching Apple Events and Watching Tech reviews </strong></li>
        <li><em>Hobbies:</em> <strong> Watching Cricket</strong></li>
        <li><em>Career Goal:</em>  <strong>Computer Scientist.</strong></li>
    </ul>
    <hr>
    <h1 style="color: Red;text-align: Center; font-size: 60px ;font-family:Georgia">Table Of Project </h1>
    <hr>
    <table  border="5"; width:"600px" ; height:"100px"; font-size:"100px">
      <tr style="background-color: #D6EEEE;">
        <th style=" font-size: 70px"> Project Title</th>
        <th style=" font-size: 70px">Description</th>
        <th style=" font-size: 70px">Completion Due</th>
      </tr>
      <tr style="background-color:#D1EFF5">
        <td style=" font-size: 50px">
          <a href="Adventure.html">Adventure Story Website</a></td>
        <td style=" font-size: 50px">In this project, I created a website that takes the user through a short computer science adventure story. </td>
        <td style=" font-size: 50px">September 5, 2023</td>
      </tr>
      <tr style="background-color: #D6EEEE;">
          <td style=" font-size: 50px"><a href="Emerging_Tech_Expert.html">Emerging Tech Expert website</a></td>
          <td style=" font-size: 50px">I'm an expert on Virtual Reality, so I made a website so others can know more about it.</td>
          <td style=" font-size: 50px">Oct 11, 2023</td>
      </tr>
    </table>
  </body>
</html>
