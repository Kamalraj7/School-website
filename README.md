<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        :root{
            --day-bg: white;
            --day-text: black;
            --night-bg: #121212;
            --night-text: #f0f0f0;
        }
        .header{
            font-size: 16px;
            background-color: aliceblue;
            margin: 0;
        }
        .header ul{
            display: flex;
            justify-content: flex-end;
            align-items: right;
            gap: 130px;

        }
        .header img{
            width: 200px;
            height: 100px;
        }
        .toggle-mode{
            display: inline-block;
            padding: 10px 20px;
            margin: 10px;
            background:aliceblue;
            color: black;
            border-radius: 8px;
        }
        .page {
            background-color: var(--day-bg);
            color: var(--day-text);
            transition: all 0.3s ease;
            padding: 20px;
        }
       
        #themeToggle:checked ~ .page {
            background-color: var(--night-bg);
            color: var(--night-text);
        }
        .home{
            display: inline-block;
            padding: 1px;
            margin: 0;
        }
        .home img{
            width: 200px;
            height: 100px;
            transition: transform 0.3s linear;
        }
        .home img:hover{
            transform: scale(1.1);
        }
        .home-logo{
            display: flex;
            background-color: aliceblue;
            gap: 200px;
        }
        .home-logo img{
            width: 50px;
            height: 50px;
        }
        .download{
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
            font-size: 16px;
        }
        .download:hover {
            background-color: aliceblue;
            transform: scale(1.05);
        }
        .more-texts{
            display: none;
        }
        .toggle-box{
            display: none;
        }
        .read-more{
            display:inline-block;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .read-more:hover{
            background-color: #0056b3;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
            font-size: 16px;
            padding: 1px;
        }
        .toggle-box:checked ~ p .more-texts {
            display: inline;
        }

        .toggle-box:checked ~ p .dots {
            display: none;
        }

        .toggle-box:checked ~ .read-more::after {
            content: " Read Less";
        }
        .About-us{
            padding: 10px;
            margin: 0 auto; 
        }
        .slider{
                width: 400px;
                height: 400px;
                margin: 0 auto;
                                
            }
            .slides{
                display: flex;
                justify-content: flex-start;
                transition: transform 0.5s ease-in-out;
            }
             .slides img{
                width: 300px;
                height: 300px;
                object-fit: cover;
            }
        .skills{
            background-color: aliceblue;
            padding: 10px;
            margin: 0 auto;
        }
        .linear-progress {
            width: 300px;
            height: 20px;
            background-color: #eee;
            border-radius: 10px;
            overflow: hidden;
        }
        .linear-fill {
            height: 100%;
            background-color: #007bff;
            width: 0;
            transition: width 0.5s ease;
        }
    .card{
        display:inline-block;
        background: white;
        border-radius: 16px;
        padding: 25px;
        box-shadow: 0 8px 20px rgba(0,0,0,0.1);
        transition: transform 0.3s, box-shadow 0.3s;
        cursor: pointer;
        width: 100%;
        max-width: 300px;
    }
    .card h2 {
    font-size: 1.3em;
    margin-bottom: 10px;
    color: #007bff;
    }
    .card h3 {
    font-size: 1.3em;
    margin-bottom: 10px;
    color: #007bff;
    }
    .card p {
        font-size: 1em;
        color: #333;
    }
    .card:hover {
  transform: translateY(-10px);
  box-shadow: 0 12px 25px rgba(0,0,0,0.2);
    }
    .btn{
                display: inline-block;
                background: #f77f00;
                padding: 0.7rem 1.5rem;
                color: white;
                border-radius: 20px;
                margin-top: 1rem;
                text-decoration: none;
                font-weight: bold;
    }
    .btn:hover{
             background-color: #0056b3;
    }
    .projects-cards{
        background-color: aliceblue;
        width: 100%;
    }
    .projects h1 {
    font-size: 2.5em;
    margin-bottom: 10px;
    color: #007bff;
    }
    .projects b {
        font-size: 1.05em;
        color: #333;
    }
    .contact{
        display: inline-block;
        background-color: aliceblue;
        font-size: 1.3em;
        margin-bottom: 10px;
        color: #007bff;
        width: 100%; 
    }
    .footer{
        display: flex;
        background-color:#0693e3 ;
        width: 100%;
    }
    
    </style>
</head>
<body>
    <header>
        <input type="checkbox" id="themeToggle" class="toggle-mode"> 
        <label for="themeToggle" class="toggle-mode">Toggle Day/Night</label>
        <div class="header">
            <img src="https://png.pngtree.com/png-vector/20221215/ourmid/pngtree-school-logo-design-png-image_6524414.png">
            <h1>XYZ School</h1>
            <ul>
                <li><a href="#Home">Home</a></li>
                <li><a href="#About-us">About us</a></li>
                <li><a href="#Skills">Skills</a></li>
                <li><a href="#Services">Services</a></li>
                <li><a href="#Contacts">Contacts</a></li>
            </ul>
       
        </div>
     <div class="page">
        <div class="home">
            <img src="https://png.pngtree.com/png-vector/20221215/ourmid/pngtree-school-logo-design-png-image_6524414.png">
            <p><h1>Welcome to XYZ School</h1>

                At XYZ School, we believe that every child has the potential to shine. Founded on the principles of excellence, inclusivity, and holistic development, our school is dedicated to nurturing young minds into confident, compassionate, and creative individuals.
                With a vibrant learning environment, experienced faculty, and a rich blend of academics, arts, and sports, we strive to provide students with the skills and values necessary to thrive in today’s world. Our curriculum is designed to foster critical thinking, curiosity, and a lifelong love of learning.
                Join us at XYZ School, where education goes beyond textbooks — shaping future leaders and responsible citizens.</p>
        
        <div class="home-logo">
            <a href="facebook"><img src="https://img.icons8.com/?size=100&id=118466&format=png&color=000000"></a>
            <a href="Whatsapp"><img src="https://img.icons8.com/?size=100&id=16712&format=png&color=000000"></a>
            <a href="Email"><img src="https://img.icons8.com/?size=100&id=12580&format=png&color=000000"></a>
            <a href="Call"><img src="https://img.icons8.com/?size=100&id=9660&format=png&color=000000"></a>
        </div>
        <div class="resume">
            <a href="path/to/yourfile.pdf" download>
                <button class="download">Download</button>
            </a>
        </div>
    <div class="About-us">
        <input type="checkbox" id="toggle-box" class="toggle-box">
        <h1>About Us</h1>
        <p>Welcome to XYZ School, a nurturing environment where education meets excellence. Founded with a vision to empower young minds through quality education, our school is committed to fostering academic curiosity, personal growth, and social responsibility.
            <span class="dots">....</span>
            <span class="more-texts">
                At XYZ School, we believe that every child is unique and holds infinite potential. Our dedicated faculty and staff work tirelessly to create an engaging and inclusive atmosphere that supports holistic development. We focus not just on academics but also on instilling strong moral values, creativity, leadership, and a lifelong love for learning.
                Our curriculum is thoughtfully designed to balance knowledge with practical skills, preparing students to excel in a rapidly changing world. Whether it's through innovative teaching methods, co-curricular activities, or community service, we strive to create well-rounded individuals who are ready to face future challenges with confidence and compassion.
                Join us on this journey of growth and transformation — where dreams are nurtured, talents are discovered, and future leaders are born.</p>
                </span>
            
            <label for="toggle-box" class="read-more">Read more </label>
        </div>
        <div class="slider">
            <div class="slides">
                <img src="https://img.freepik.com/free-vector/four-happy-kids-with-backpacks-green-hill_9975-108628.jpg?semt=ais_hybrid&w=740">
                <img src="https://img.freepik.com/premium-vector/children-going-school_1639-42108.jpg">
                <img src="https://img.freepik.com/premium-vector/happy-school-children-front-school_29190-5231.jpg">
            </div>
        </div>

    <div class="skills-section">
            <h1>Skills</h1>
            <div class="skills-cards">
                <div class="card">
                <h3>Mastery</h3>
                <p>Strong foundation in science, mathematics, languages, and social studies.</p>
                </div>
                <div class="card">
                <h3>Communication Skills</h3>
                <p>Enhancing reading, writing, speaking, and listening abilities.</p>
                </div>
                <div class="card">
                <h3>Critical Thinking & Problem Solving</h3>
                <p>Encouraging analytical thinking through experiments, debates, and interactive lessons.</p>
                </div>
                <div class="card">
                <h3>Creativity and Innovation</h3>
                <p>Fostering imagination and artistic expression through arts, music, and creative writing.</p>
                </div>
                <div class="card">
                <h3>Digital Literacy</h3>
                <p>Building competence in technology usage, coding basics, and safe internet practices.</p>
                </div>
                <div class="card">
                <h3>Leadership & Teamwork</h3>
                <p>Activities, clubs, and councils develop collaboration and leadership qualities.</p>
                </div>
                <div class="card">
                <h3>Physical & Emotional Well-being</h3>
                <p>Promoting sports, yoga, and mindfulness for holistic health.</p>
                </div>
            </div>
</div>

    <div class="linear-progress">
        <div class="linear-fill" style="width: 50%;"></div>
    </div>  
    <div class="certifications">
        <h1>Certifications</h1>

            Our certification offerings include:<br>
          <!-- Academic Certifications Card -->
            <div class="card">
            <h2>Academic Certifications</h2>
            <p>Acknowledging exceptional performance in core subjects like Mathematics, Science, and Languages.</p>
            <a href="certificates/academic.pdf" target="_blank" class="btn">View Certificate</a>
            </div>

            <!-- Digital Skills Certifications Card -->
            <div class="card">
            <h2>Digital Skills Certifications</h2>
            <p>Verifying proficiency in computer literacy, coding fundamentals, and online safety.</p>
            <a href="certificates/digital_skills.pdf" target="_blank" class="btn">View Certificate</a>
            </div>

            <!-- Leadership Certifications Card -->
            <div class="card">
            <h2>Leadership Certifications</h2>
            <p>Recognizing abilities in communication, teamwork, and leadership roles within school activities.</p>
            <a href="certificates/leadership.pdf" target="_blank" class="btn">View Certificate</a>
            </div>

            <!-- Creative Arts Certifications Card -->
            <div class="card">
            <h2>Creative Arts Certifications</h2>
            <p>Celebrating accomplishments in arts, music, drama, and creative writing.</p>
            <a href="certificates/creative_arts.pdf" target="_blank" class="btn">View Certificate</a>
            </div>

            <!-- Health and Safety Certifications Card -->
            <div class="card">
            <h2>Health and Safety Certifications</h2>
            <p>Ensuring awareness and skills in first aid, wellness, and safe practices.</p>
            <a href="certificates/health_safety.pdf" target="_blank" class="btn">View Certificate</a>
            </div>

            <!-- Sports and Fitness Certifications Card -->
            <div class="card">
            <h2>Sports and Fitness Certifications</h2>
            <p>Highlighting achievements and participation in various sports and physical education programs.</p>
            <a href="certificates/sports_fitness.pdf" target="_blank" class="btn">View Certificate</a>
            </div> 
        <div class="projects-section">
  <h1>Projects</h1>
  <p>
    At XYZ School, we encourage our students to learn by doing. Our project-based learning approach fosters curiosity, creativity, and practical understanding.
  </p>

  <div class="project-cards">

    <div class="card">
      <h3>Science and Innovation</h3>
      <p>Students explore real-world scientific problems through model making, experiments, and science fairs.</p>
    </div>

    <div class="card">
      <h3>Environmental Projects</h3>
      <p>Tree plantation drives, waste segregation awareness, and eco-friendly models promoting sustainability.</p>
    </div>

    <div class="card">
      <h3>Math in Daily Life</h3>
      <p>Projects show how math applies to budgeting, measurement, construction, and logical reasoning.</p>
    </div>

    <div class="card">
      <h3>Digital & Coding</h3>
      <p>App prototypes, basic programming, and multimedia presentations to build tech skills.</p>
    </div>

    <div class="card">
      <h3>Social Awareness</h3>
      <p>Topics like gender equality, cleanliness, and civic duties presented via posters and campaigns.</p>
    </div>

    <div class="card">
      <h3>Art-Integrated Projects</h3>
      <p>Projects blending academics with drawing, music, and creative expression for multi-sensory learning.</p>
    </div>

<div class="contact">
    <h1>Contacts</h1>
    <input text="name" placeholder="name">
    <input text="email" placeholder="name@gmail.com">
    <input text="message input" placeholder="message">
    <button class="download">Submit</button>
</div>
</header>

<footer  class="footer">
    <p>&copy;2025 XYZ School. All rights reserved.</p>
    <div class="Social">
        <a href="facebook"><img src="https://img.icons8.com/?size=100&id=118466&format=png&color=000000"><button class="download">Facebook</button></a>
        <a href="Whatsapp"><img src="https://img.icons8.com/?size=100&id=16712&format=png&color=000000"><button class="download">Whatsapp</button></a>
        <a href="Email"><img src="https://img.icons8.com/?size=100&id=12580&format=png&color=000000"><button class="download">Email</button></a>
        <a href="Call"><img src="https://img.icons8.com/?size=100&id=9660&format=png&color=000000"><button class="download">Call</button></a>
        
        
    </div>

</footer>
    
</body>
</html>
