# Styled_Profile_Card
## Date: 8/7/25

## Objective:
To practice HTML and CSS fundamentals by designing a visually appealing profile card that demonstrates the use of background color, typography, spacing, and layout alignment techniques.

## Tasks:
#### 1. Create the HTML Structure:
Use ```<!DOCTYPE html>, <html>, <head>, and <body>``` to define the structure.
Add a ```<title>``` like "My Profile Card".

#### 2. Add Content:
Include name, title (e.g., Developer, Student), and a short bio using semantic tags such as ```<h1>```, ```<h2>```, and ```<p>```.

#### 3. Add a Profile Image:
Use the ```<img>``` tag to include a profile picture with appropriate alt, width, and height attributes.

#### 4. Apply Background Color:
Use a CSS class to style the card with a background color.

#### 5. Style Typography:
Use CSS to apply different font families, sizes, and text colors for the name and bio.

#### 6. Add Spacing:
Apply margin and padding to improve spacing between elements using CSS.

#### 7. Center the Card:
Use flexbox or margin: auto to center the card vertically and horizontally on the page.

#### 8. Add Hover Effects:
Enhance interactivity with simple hover effects like border changes or background transition using CSS.

## HTML Code:
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Profile - Praveena N</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="profile-card">
        <img src="pic.jpg" alt="Praveena N">
        <h1>Praveena N</h1>
        <h2>Aspiring Software Engineer</h2>
    </div>

    <section>
        <h3>Contact Information</h3>
        <p>Email: praveena22062005@gmail.com</p>
        <p>Phone: 8838216220</p>
        <p>Location: Chennai, India</p>
        <p>LinkedIn: <a href="https://www.linkedin.com/in/praveena-n-a2434a251">linkedin.com/in/praveena-n-a2434a251</a></p>
    </section>

    <hr>

    <section>
        <h3>About Me</h3>
        <p>
            I am a passionate and detail-oriented Computer Science student with strong skills in design and problem-solving.
            I enjoy building web applications and transforming ideas into real-world solutions. I’m eager to work in a challenging environment that helps me grow both personally and professionally.
        </p>
    </section>

    <hr>

    <section>
        <h3>Education</h3>
        <ul>
            <li><strong>BE Computer Science and Engineering</strong> – Saveetha Engineering College, CGPA: 8.4 (2022 - Present)</li>
            <li><strong>HSC</strong> – The Path Global Public School, 74%</li>
            <li><strong>SSC</strong> – The Path Global Public School, 83.2%</li>
        </ul>
    </section>

    <hr>

    <section>
        <h3>Projects</h3>
        <ul>
            <li><strong>CollegeQuest</strong> – A MERN stack platform to help students choose colleges based on their interests.</li>
            <li><strong>Spotify Clone</strong> – A responsive music website using React.js and Tailwind CSS.</li>
            <li><strong>Weather Forecast App</strong> – A real-time weather app using the MERN stack.</li>
        </ul>
    </section>

    <hr>

    <section>
        <h3>Work Experience</h3>
        <p><strong>Web Developer Intern</strong> – Arjun Vision Tech Solutions (June 2024 – July 2024)</p>
        <ul>
            <li>Developed responsive web apps using HTML, CSS, JavaScript.</li>
            <li>Collaborated with a team to build dynamic web pages.</li>
        </ul>
    </section>

    <hr>

    <section>
        <h3>Skills</h3>
        <p>
            HTML, CSS, JavaScript, Java, React.js, Node.js, Express.js, MongoDB, GitHub
        </p>
    </section>

    <hr>

    <section>
        <h3>Achievements & Competitions</h3>
        <ul>
            <li>1st Prize - Quiz (ORKESTRIM'24, SRM Valliammai Engineering College)</li>
            <li>IBM Z Datathon - Participant (2023, 2024)</li>
            <li>Crypt Hunt - SAMHITA'24, MIT</li>
            <li>Tech Events - SPECTRON'24, BS Crescent Institute</li>
            <li>GDSC Compose Camp - Intro to Android Development (Kotlin)</li>
        </ul>
    </section>

    <hr>

    <section>
        <h3>Certifications</h3>
        <ul>
            <li>AWS Cloud Practitioner – ICT Academy</li>
            <li>Industrial IoT – NPTEL</li>
            <li>Google Cloud Career Launchpad – Google</li>
            <li>Developing Front-End Apps with React – IBM (Coursera)</li>
        </ul>
    </section>

</body>
</html>
```
```
style.css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(to right, lightcyan, lightblue);
    color: #0d47a1;
    line-height: 1.6;
    padding: 20px;
    max-width: 900px;
    margin: auto;
}

.profile-card {
    background-color: white;
    padding: 30px 20px;
    text-align: center;
    border-radius: 16px;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
    margin-bottom: 40px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.profile-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 28px rgba(0, 0, 0, 0.15);
}

.profile-card img {
    width: 140px;
    height: 140px;
    object-fit: cover;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 5px solid skyblue;
}

.profile-card h1 {
    font-size: 2.2em;
    margin-bottom: 5px;
    color: #1565c0;
}

.profile-card h2 {
    font-size: 1.2em;
    color: #2980b9;
    font-weight: normal;
}


section {
    background: white;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.06);
}

h3 {
    font-size: 1.2em;
    color: #1a5276;
    margin-bottom: 12px;
}

p, li {
    font-size: 1em;
    margin-bottom: 8px;
}

ul {
    padding-left: 20px;
}

a {
    color: #1e88e5;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

hr {
    border: none;
    border-top: 1px solid #ccc;
    margin: 30px 0;
}

@media (max-width: 600px) {
    .profile-card img {
        width: 100px;
        height: 100px;
    }

    .profile-card h1 {
        font-size: 1.6em;
    }

    .profile-card h2 {
        font-size: 1em;
    }
}
```

## Output:
![image](https://github.com/user-attachments/assets/2ede360d-ad96-4229-b271-0ebee9f7042f)
![image](https://github.com/user-attachments/assets/1a944f8a-cd25-48c8-8805-19c2b3267e55)
![image](https://github.com/user-attachments/assets/85d57b4f-565e-4cad-9fa4-1f84dd4f6c6c)
![image](https://github.com/user-attachments/assets/d8861d99-d0a7-4cc8-a5a6-0383eaeb2491)


## Result:
A visually appealing profile card that demonstrates the use of background color, typography, spacing, and layout alignment techniques is designed.
