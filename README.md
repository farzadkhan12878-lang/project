<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Navbar</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            min-height: 100vh;
            font-family: Arial, sans-serif;
            background: linear-gradient(120deg, #123f91, #071b50, #28145c);
            color: white;
        }

        h1 {
            text-align: center;
            margin-top: 55px;
            font-size: 45px;
        }

        h1 span {
            color: #48c8ff;
            font-size: 55px;
        }

        .navbar {
            width: 80%;
            height: 85px;
            margin: 135px auto 0;
            padding: 0 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;

            background: rgba(255, 255, 255, 0.15);
            border: 1px solid rgba(255, 255, 255, 0.35);
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 22px;
            font-weight: bold;
        }

        .logo-circle {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            background: linear-gradient(135deg, #39c5ff, #707cff);
        }

        .links {
            display: flex;
            gap: 45px;
            list-style: none;
        }

        .links a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }

        .signup {
            border: none;
            padding: 15px 27px;
            border-radius: 13px;
            color: white;
            font-size: 17px;
            font-weight: bold;
            background: linear-gradient(90deg, #35c5f5, #7c83ef);
        }

        .mobile-navbar {
            display: none;
        }

        @media (max-width: 700px) {

            h1 {
                font-size: 25px;
                margin-top: 40px;
            }

            h1 span {
                font-size: 32px;
            }

            .navbar {
                display: none;
            }

            .mobile-navbar {
                width: 70%;
                height: 75px;
                margin: 120px auto 0;
                padding: 0 25px;

                display: flex;
                align-items: center;
                justify-content: space-between;

                background: rgba(255, 255, 255, 0.15);
                border: 1px solid rgba(255, 255, 255, 0.35);
                border-radius: 18px;
                backdrop-filter: blur(10px);
            }

            .menu {
                width: 38px;
            }

            .menu div {
                height: 3px;
                margin: 7px 0;
                background: white;
                border-radius: 5px;
            }
        }
    </style>
</head>

<body>

    <h1>
        <span>20</span> CSS Responsive Navbar Designs
    </h1>

    <!-- Desktop Navbar -->
    <nav class="navbar">

        <div class="logo">
            <div class="logo-circle"></div>
            Flow
        </div>

        <ul class="links">
            <li><a href="#">Home</a></li>
            <li><a href="#">Product</a></li>
            <li><a href="#">Docs</a></li>
            <li><a href="#">Blog</a></li>
        </ul>

        <button class="signup">Sign up</button>

    </nav>


    <!-- Mobile Navbar -->
    <nav class="mobile-navbar">

        <div class="logo">
            <div class="logo-circle"></div>
            Flow
        </div>

        <div class="menu">
            <div></div>
            <div></div>
            <div></div>
        </div>

    </nav>

</body>
</html>

