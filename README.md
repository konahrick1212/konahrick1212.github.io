<meta name="keywords" content="Brandon Mullins">
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Scholarship Application Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-image: url('colacat.jpg'); /* Replace 'background.jpg' with the path to your background image */
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            padding: 0;
            margin: 0;
        }
        
        header {
            padding: 20px 0;
        }

        main {
            padding: 20px;
            text-align: left;
            max-width: 800px;
            margin: 0 auto;
            background-color: rgba(255, 255, 255, 1); /* Set background color to solid white */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3); /* Add a subtle shadow for depth */
            border-radius: 10px; /* Add border radius for rounded corners */
            overflow: hidden; /* Prevent content overflow */
        }

        section {
            margin-bottom: 20px;
            position: relative; /* Set position relative to allow positioning of the pillar */
        }

        h2 {
            cursor: pointer;
            background-color: #f0f0f0;
            padding: 10px;
            margin: 0;
        }

        p {
            margin-top: 0;
        }

        .content {
            display: none;
            padding: 10px;
        }

        .active {
            display: block;
        }

        .pillar {
            position: absolute;
            width: 40px;
            height: 500%;
            background-color: #fff; /* Set background color to solid white */
            left: -5px;
            top: 0;
            z-index: -2;
        }

        .cat-image {
            max-width: 200px;
            margin: 10px auto;
            display: block;
        }

        .info-box {
            background-color: #fff;
            padding: 10px;
            margin-bottom: 20px;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.3); /* Add a shadow for depth */
            display: inline-block; /* Ensure it wraps around the content */
        }
    </style>
</head>
<body>

    <header>
        <div class="info-box">
            <h1>Brandon Mullins</h1>
            <p>Contact: mullinsbrandon885@gmail.com | Phone: 269-464-6816</p>
        </div>
    </header>

    <main>
        <section id="about">
            <h2>About Me</h2>
            <div class="pillar"></div> <!-- Add a white pillar behind the text -->
            <div class="content">
                <p>I am a College Student who is majoring in computer science with a particular interest in cybersecurity and penetration testing.</p>
                <p>My hobbies include but are not limited to gaming, various personal projects (usually involving cybersecurity or computers and electronics in general), cooking, and playing Dungeons and dragons with my friends.</p>
            </div>
        </section>

        <section id="achievements">
            <h2>Achievements</h2>
            <div class="pillar"></div>
            <div class="content">
                <ul>
                    <li>Several Certifications pertaining to IT such as</li>
                    <li>Microsoft Technology Associate (MTA) Security Fundamentals</li>
                    <li>MTA Windows OS fundamentals</li>
                    <li>TestOut IT fundamentals</li>
                    <li>TestOut Online Safety and Security</li>
                    <li>TestOut IT fundamentals</li>
                    <li>TestOut Security</li>
                    <li>TestOut Ethical Hacking</li>
                    <li>A less formal Achievement of mine is jailbreaking a locked down control module for a robotics competition. Allowing it to be used after the competition was over.</li>
                </ul>
            </div>
        </section>

        <section id="extracurricular">
            <h2>Extracurricular Activities</h2>
            <div class="pillar"></div>
            <div class="content">
                <ul>
                    <li>Playing Dungeons and Dragons with my friends</li>
                    <li>Reading up on Cybersecurity related topics (news, software, etc)</li>
                    <li>Coding various programs or scripts.</li>
                </ul>
            </div>
        </section>

        <section id="cats">
            <h2>My Cats</h2>
            <div class="pillar"></div>
            <div class="content">
                <div>
                    <h3>Finn</h3>
                    <img class="cat-image" src="finn.jpg" alt="Picture of Finn being Smug">
                    <img class="cat-image" src="finn2.jpg" alt="Finn taking a nap">
                </div>
                <div>
                    <h3>Hadrian</h3>
                    <img class="cat-image" src="hadrian.jpg" alt="Picture of Hadrien seeing what im doing">
                    <img class="cat-image" src="hadrian2.jpg" alt="Hadrian judging you">
                </div>
                <div>
                    <h3>Ocatavia</h3>
                    <img class="cat-image" src="octavia.jpg" alt="Picture of Octavia getting ready to strike">
                    <img class="cat-image" src="octavia2.jpg" alt="Octavia also judging you">
                </div>
            </div>
        </section>

        <section id="goals">
            <h2>Career Goal</h2>
            <div class="pillar"></div>
            <div class="content">
                <p>My Career goal overall is to get into the cybersecurity field of IT and continue to develop my skills both career wise as well as for my hobbies.</p>
            </div>
        </section>
    </main>

    <footer>
        <p>Contact: mullinsbrandon885@gmail.com | Phone: 269-464-6816</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            var sections = document.querySelectorAll('section');

            sections.forEach(function(section) {
                var header = section.querySelector('h2');

                header.addEventListener('click', function() {
                    sections.forEach(function(s) {
                        if (s !== section) {
                            s.querySelector('.content').classList.remove('active');
                        }
                    });

                    section.querySelector('.content').classList.toggle('active');
                });
            });
        });
    </script>

</body>
</html>
