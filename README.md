<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Sahib Hussain Portfolio</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background: linear-gradient(135deg,#0f172a,#1e293b,#7c3aed);
    color:white;
    overflow-x:hidden;
}

/* Animated Background */
.bg{
    position:fixed;
    width:100%;
    height:100%;
    overflow:hidden;
    z-index:-1;
}

.bg span{
    position:absolute;
    display:block;
    width:25px;
    height:25px;
    background:rgba(255,255,255,0.08);
    animation: animate 20s linear infinite;
    bottom:-150px;
    border-radius:50%;
}

.bg span:nth-child(1){left:10%; width:80px; height:80px; animation-delay:0s;}
.bg span:nth-child(2){left:25%; animation-delay:2s;}
.bg span:nth-child(3){left:40%; width:60px; height:60px; animation-delay:4s;}
.bg span:nth-child(4){left:55%; animation-delay:0s;}
.bg span:nth-child(5){left:70%; width:90px; height:90px; animation-delay:3s;}
.bg span:nth-child(6){left:85%; animation-delay:7s;}

@keyframes animate{
    0%{
        transform:translateY(0) rotate(0deg);
        opacity:1;
    }
    100%{
        transform:translateY(-1000px) rotate(720deg);
        opacity:0;
    }
}

.container{
    width:90%;
    max-width:1100px;
    margin:auto;
    padding:40px 0;
}

/* Hero Section */
.hero{
    display:flex;
    flex-wrap:wrap;
    align-items:center;
    justify-content:space-between;
    min-height:100vh;
}

.hero-text{
    flex:1;
    animation:slideLeft 1.5s ease;
}

.hero-text h1{
    font-size:65px;
    line-height:75px;
    font-weight:700;
}

.hero-text h1 span{
    color:#facc15;
}

.hero-text p{
    margin-top:20px;
    font-size:18px;
    color:#d1d5db;
    max-width:500px;
}

.btn{
    display:inline-block;
    margin-top:30px;
    padding:14px 30px;
    background:#f43f5e;
    color:white;
    text-decoration:none;
    border-radius:40px;
    font-weight:600;
    transition:0.4s;
    box-shadow:0 0 20px rgba(244,63,94,0.5);
}

.btn:hover{
    transform:scale(1.1);
    background:#e11d48;
}

.hero-img{
    flex:1;
    text-align:center;
    animation:float 3s ease-in-out infinite;
}

.hero-img img{
    width:320px;
    border-radius:30px;
    border:5px solid rgba(255,255,255,0.2);
    box-shadow:0 0 30px rgba(255,255,255,0.2);
}

@keyframes float{
    0%,100%{
        transform:translateY(0);
    }
    50%{
        transform:translateY(-20px);
    }
}

@keyframes slideLeft{
    from{
        opacity:0;
        transform:translateX(-80px);
    }
    to{
        opacity:1;
        transform:translateX(0);
    }
}

/* Cards */
.section{
    margin-top:60px;
}

.section-title{
    font-size:40px;
    margin-bottom:30px;
    text-align:center;
    color:#facc15;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.card{
    background:rgba(255,255,255,0.08);
    padding:30px;
    border-radius:25px;
    backdrop-filter:blur(10px);
    transition:0.4s;
    border:1px solid rgba(255,255,255,0.1);
}

.card:hover{
    transform:translateY(-10px) scale(1.03);
    background:rgba(255,255,255,0.12);
}

.card h3{
    margin-bottom:15px;
    color:#f472b6;
}

.card ul{
    padding-left:20px;
    color:#e5e7eb;
}

/* Footer */
footer{
    text-align:center;
    padding:40px 20px;
    margin-top:50px;
    color:#d1d5db;
}

@media(max-width:768px){

.hero{
    flex-direction:column-reverse;
    text-align:center;
}

.hero-text h1{
    font-size:45px;
    line-height:55px;
}

.hero-img img{
    width:250px;
    margin-bottom:30px;
}

}
</style>
</head>
<body>

<div class="bg">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
</div>

<div class="container">

    <!-- Hero -->
    <section class="hero">

        <div class="hero-text">
            <h1>Hi, I'm <span>Sahib Hussain</span></h1>

            <p>
                Motivated and hardworking fresher seeking an opportunity 
                to start my career and grow professionally. 
                Passionate to learn new skills and achieve success.
            </p>

            <a href="#" class="btn">Hire Me</a>
        </div>

        <div class="hero-img">
            <img src="https://i.ibb.co/6rTHSCp/user.png" alt="profile">
        </div>

    </section>

    <!-- Skills -->
    <section class="section">
        <h2 class="section-title">My Skills</h2>

        <div class="cards">

            <div class="card">
                <h3>Computer Skills</h3>
                <ul>
                    <li>Basic Computer Knowledge</li>
                    <li>Internet Browsing</li>
                    <li>MS Office Basics</li>
                </ul>
            </div>

            <div class="card">
                <h3>Communication</h3>
                <ul>
                    <li>Hindi</li>
                    <li>English</li>
                    <li>Punjabi</li>
                </ul>
            </div>

            <div class="card">
                <h3>Personality</h3>
                <ul>
                    <li>Quick Learner</li>
                    <li>Hardworking</li>
                    <li>Punctual</li>
                </ul>
            </div>

        </div>
    </section>

    <!-- Education -->
    <section class="section">
        <h2 class="section-title">Education</h2>

        <div class="cards">

            <div class="card">
                <h3>12th Pass</h3>
                <p>Higher Secondary Education Completed.</p>
            </div>

            <div class="card">
                <h3>Experience</h3>
                <p>Fresher looking for opportunities to grow professionally.</p>
            </div>

            <div class="card">
                <h3>Contact</h3>
                <p>📞 +91 7986390414</p>
                <p>✉️ sahibhussain593@gmail.com</p>
            </div>

        </div>
    </section>

</div>

<footer>
    © 2026 Sahib Hussain | Personal Portfolio Website
</footer>

</body>
</html>
