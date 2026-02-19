<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>intoduction web</title>
    <link rel="stylesheet" href="intro.css">
    <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"
  />
</head>
<body>
    <style>
        *, html, body{
    margin: 0;
    padding: 0;
    font-family: Helvetica;
    scroll-behavior: smooth;
}


header {
    background-color: #1A2238;
    color: #eaeaea;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 10px;
}


.logo{
    margin-right : auto;
    margin-left: 10px;
    cursor: pointer;
    transition: all .5s ease 0s;
}

.logo:hover {
    color:#FF6A3D;
    transform: rotate(2deg);
}

a {
    color: #eaeaea;
    text-decoration: none;
    
}

nav ul {
    display: flex;
    padding: 20px;
}

li {
    list-style-type: none;
    padding: 10px;
}

li a {
     transition: all .5s ease 0s;
     display: inline-block;
}

li a:hover {
    color:#FF6A3D;
     transform: rotate(2deg);
    
}

.btn-cta {
    margin-right: 10px;
    border:none;
    font-size: 20px;
    padding: 6px 12px;
    background: #FF6A3D;
    color: #eaeaea;
    border-radius: 8px;
    cursor: pointer;
}

.container  {
    max-width: 1200px;
    margin: 0 auto;
    padding: 70px 0;
}

.intro {
    display: flex;
    flex-direction: column; 
    justify-content: center;
    align-items: center;
    gap: 10px;
    text-align: center;
}

.title {
    font-size: 24px;
    font-weight: bold;
}

.description {
    font-size: 28px;
    font-weight: bolder;
}

.img-photo {
    max-width: 500px;
    width: 100%;
    height: auto;
    padding: 10px;
}

.content {
    background-image: url(WhatsApp\ Image\ 2026-02-19\ at\ 20.20.54.jpeg);
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
   background-size: cover;
   height: 145vh;
}

.tentang {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: #1A2238;
    color: #eaeaea;
    padding: 40px;

}

.mt-10 {
    margin-top: 20px;
}
.card {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 8px;
}

.card-item {
    text-align: center;
    width: 20%;
    min-height: 200px;
    max-height: 300px;
    background: #f7f7f7;
    color: #222;
    padding: 24px;
    box-shadow: 2px 5px 5px 1px rgba(0, 0, 0, 0.5);
}

.icon {
 width: 75px;
 height: 75px;
 margin: 10px;
 padding: 4px;
}

.card-title {
    font-size: 20px;
    font-weight: bolder;
}

.card-description {
    font-size: 14px;
    margin-top: 4px;
}


@media screen  and  ( max-width : 500px) {

    .card {
        flex-direction: column;
        gap: 0;
    }

    .card-item {
        width: 100%;
        opacity: 0.9;
    }

   .container {
    max-width: 100%;
    padding: 0;
   }

   .intro {
    margin-top: 20px;
   }

   .img-photo {
    padding: 0;
   }

   nav {
    position: fixed;
    bottom: 0;
    width: 100%;
    background: #1A2238;
    z-index: 9;
    }

    footer {
        margin-bottom: 60px;
        margin-top: 10px;
    }
   

}

footer {
    padding: 20px;
    text-align: center;
    background: #1A2238;
    color: #eaeaea;
}


    </style>
    <header class="animate__animated animate__pulse">
        <h1 class="logo">requilme</h1>
        <nav>
            <ul>
                <li><a href="#jasa">JASA</a></li>
                <li><a href="mailto:sancode@icloud.com">CONTACT</a></li>
            </ul>
        </nav>
        <button class="btn-cta" onclick="redir()">Follow saya</button>
    </header>
    <div class="container">
        <div class="intro">
            <p   class="title animate__animated animate__backInLeft" >Hello, Requilme Here!</p>
            <p class="description animate__animated animate__backInRight">Techonolgy developer from influencer</p>
            <img class="img-photo animate__animated animate__backInUp animate__delay-2s" src="8ca56409-0275-4879-91b6-0c87733f881c.jpg" alt="">
        </div>
    </div>
    <div class="content">
        <div class="tentang">
            <p class="title">Hello, im programer</p>
            <p class="description">Mulai aja dulu jago nya ngikut.</p>
            <div class="mt-10">
                 <button class="btn-cta" onclick="redirWhatsapp()">Mari kerjasama</button>
            </div>
        </div>
        <div id="jasa" class="container">
            <div  class="card">
            <div class="card-item">
            <img class="icon" src="engineering-school-logo-design_142989-1438.avif" alt="">
             <p class=" card-title">Web developer</p>
            <p class="card-description">Saya cukup ahli dalam bidang web-developer</p>
                </div>
                <div class="card-item">
                    <img  class="icon" src="download (2).webp" alt="">
             <p class="card-title">Network</p>
            <p class=" card-description">Saya juga bisa dalam setting network</p>
                </div>
                <div class="card-item">
                    <img class="icon" src="c2f91b_630a184664b24c56b75dcc78ab43bc03~mv2.avif" alt="">
             <p class="card-title">Cisco</p>
            <p class="card-description">Pengelolahan jaringan adalah jurusan saya saat smk</p>
                </div>
            </div>
        </div>
    </div>
    <footer>
        <p class="title">&copy; requilme website 2026</p> 
    </footer>

    <script>
        function redir() {
            window.location.href = "https://instagram.com/sanrequilme"
 }
        function redirWhatsapp(){
            window.location.href ="https://wa.me/+62853152516"
        }
       
    </script>
</body>
</html>


