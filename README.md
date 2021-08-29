<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Profile Card</title>
    <style>
        body {
            margin: 0;
            font-family: tahoma;
            height: 100vh;
            background: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .card {
            padding: 30px 0 55px;
            margin-bottom: 30px;
            background-color: #f5f5f5;
            text-align: center;
            overflow: hidden;
            position: relative;
            box-shadow: 20px 20px 42px #d0d0d0, -20px -20px 42px #ffffff;
            width: 25%;
        }

        .card .picture {
            display: inline-block;
            height: 130px;
            width: 130px;
            z-index: 1;
            position: relative;
            border-radius: 20%;
        }

        .card .picture::before {
            content: "";
            width: 100%;
            height: 0;
            border-radius: 50%;
            background-color: #1f1b1b;
            position: absolute;
            bottom: 135%;
            right: 0;
            left: 0;
            opacity: 0.9;
            transform: scale(3);
            transition: all 0.3s linear 0s;
        }

        .card:hover .picture::before {
            height: 100%;
        }

        .card .picture::after {
            content: "";
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background-color: #1f1b1b;
            position: absolute;
            top: 0;
            left: 0;
            z-index: -1;
        }

        .card .picture img {
            width: 70%;
            height: auto;
            border-radius: 50%;
            transform: scale(1);
            transition: all 0.9s ease 0s;
        }

        .card:hover .picture img {
            box-shadow: 0 0 0 14px #f7f5ec;
            transform: scale(0.7);
        }

        .card .title {
            display: block;
            font-size: 15px;
            color: #1f1b1b;
            text-transform: capitalize;
            margin: 5px 37px 0;
        }

        .card .main-content {
            margin-bottom: -19px;
        }

        .card .main-content .name {
            padding: 0;
            margin: 8px;
            text-transform: uppercase;
        }

        .card .social {
            width: 100%;
            padding: 0;
            margin: 0;
            background-color: #1f1b1b;
            position: absolute;
            bottom: -100px;
            left: 0;
            transition: all 0.5s ease 0s;
        }

        .card:hover .social {
            bottom: 0;
        }

        .card .social li {
            display: inline-block;
        }

        .card .social li a {
            display: block;
            padding: 10px;
            font-size: 17px;
            color: white;
            transition: all 0.3s ease 0s;
            text-decoration: none;
        }

        .card .social li a:hover {
            color: #3e3b44;
            background-color: #f7f5ec;
            transition: 0.5s;
        }


        .skills {
            text-align: left;
            padding: 15px;
        }

        .skills ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        .skills ul li {
            border: 1px solid #1f1b1b;
            border-radius: 2px;
            display: inline-block;
            font-size: 12px;
            margin: 0 7px 7px 0;
            padding: 7px;
        }

        .skills ul li:hover {
            background: #1f1b1b;
            color: #fff;
            cursor: pointer;
            transition: 0.5s;
        }
    </style>
</head>

<body>
    <div class="card">
        <div class="picture">
            <img class="img-fluid" src="Vinayak.jpg">
        </div>
        <div class="main-content">
            <h3 class="name">Vinayak Mandare</h3>
            <span><i class="fab fa-instagram"></i>Vinayak Mandare</span>
            <h4 class="title">Frontend developer 👨‍💻</h4>
        </div>
        <ul class="social">
            <li><a href="#" class="fa fa-github"></a></li>
            <li><a href="#" class="fa fa-twitter"></a></li>
            <li><a href="#" class="fa fa-instagram"></a></li>
            <li><a href="#" class="fa fa-telegram"></a></li>
        </ul>
        <div class="skills">
            <h6>Skills</h6>
            <ul>
                <li>HTML</li>
                <li>CSS</li>
                <li>SASS</li>
                <li>JavaScript</li>
                <li>React</li>
                <li>Github</li>
                <li>Git</li>
                <li>VS code</li>
            </ul>
        </div>
    </div>

    <script src="https://kit.fontawesome.com/dd8c49730d.js" crossorigin="anonymous"></script>
</body>

</html>
