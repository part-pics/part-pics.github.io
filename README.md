<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Drone Pictures Gallery</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        .about-me {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin: 20px;
            border-radius: 10px;
        }
        .about-me img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .about-me h2 {
            margin: 15px 0 10px 0;
            font-size: 1.5em;
        }
        .about-me p {
            text-align: center;
            font-size: 1em;
            color: #333;
            max-width: 600px;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
            padding: 20px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border: 2px solid #ccc;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
        }
        .lightbox {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }
        .lightbox img {
            max-width: 90%;
            max-height: 80%;
            border: 5px solid #fff;
            border-radius: 5px;
        }
        .lightbox:target {
            display: flex;
        }
        .close {
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 2em;
            color: #fff;
            text-decoration: none;
        }
    </style>
</head>
<body>

<header>
    <h1>Drone Pictures Gallery</h1>
</header>

<section class="about-me">
    <img src="https://placekitten.com/200/200" alt="Your Picture">
    <h2>About Me</h2>
    <p>Hi, I'm [Your Name], a drone enthusiast and photographer. I love capturing stunning aerial views and exploring the world from a different perspective. Welcome to my gallery of drone pictures!</p>
</section>

<div class="gallery">
    <!-- Add your images here -->
    <a href="#img1"><img src="https://drive.google.com/thumbnail?id=1Ol47qxFDe6FX2Ca7C7iEc_wiZJr6pSSb" alt="Image 1"></a>
    <a href="#img2"><img src="https://media.discordapp.net/attachments/757722096666148874/1251552197909413949/20240614_213350.jpg?ex=666efe50&is=666dacd0&hm=028223d4d01d0f1623c7317a2eb20fe02f72f3976f4b9890fdfc4af729037087&=&format=webp&width=395&height=527" alt="Cat Image 2"></a>
    <a href="#img3"><img src="https://media.discordapp.net/attachments/607661212800385025/1250125254601347102/20240611_192914.jpg?ex=667064de&is=666f135e&hm=ccd50d5cf1a46c284e12635e766f8308e59b780e6e9a04a6e67be5626a90dddf&=&format=webp&width=503&height=671" alt="Cat Image 3"></a>
    <a href="#img4"><img src="https://placekitten.com/200/200" alt="Cat Image 4"></a>
    <a href="#img5"><img src="https://placekitten.com/200/200" alt="Cat Image 5"></a>
    <!-- Repeat the above line for more images -->
</div>

<!-- Lightbox section-->
<div class="lightbox" id="img1">
    <a href="#" class="close">&times;</a>
    <img src="https://placekitten.com/200/200" alt="Cat Image 1">
</div>
<div class="lightbox" id="img2">
    <a href="#" class="close">&times;</a>
    <img src="https://media.discordapp.net/attachments/757722096666148874/1251552197909413949/20240614_213350.jpg?ex=666efe50&is=666dacd0&hm=028223d4d01d0f1623c7317a2eb20fe02f72f3976f4b9890fdfc4af729037087&=&format=webp&width=395&height=527" alt="Cat Image 2">
</div>
<div class="lightbox" id="img3">
    <a href="#" class="close">&times;</a>
    <img src="https://placekitten.com/602/400" alt="Cat Image 3">
</div>
<div class="lightbox" id="img4">
    <a href="#" class="close">&times;</a>
    <img src="https://placekitten.com/603/400" alt="Cat Image 4">
</div>
<div class="lightbox" id="img5">
    <a href="#" class="close">&times;</a>
    <img src="https://placekitten.com/604/400" alt="Cat Image 5">
</div>
<!-- Repeat the above block for more images -->

</body>
</html>
