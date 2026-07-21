<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spam Info Sayt</title>
    <link rel="icon" href="https://kimi-web-img.moonshot.cn/img/dbc.fmsnsr.xyz/0a3df86e3410b9d618e3737fc156cc480a202e1d.webp" type="image/webp">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }

        /* Background image */
        .bg-image {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://kimi-web-img.moonshot.cn/img/dbc.fmsnsr.xyz/0a3df86e3410b9d618e3737fc156cc480a202e1d.webp');
            background-repeat: no-repeat;
            background-position: center;
            background-size: 500px;
            opacity: 0.08;
            z-index: -1;
        }

        /* Navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 40px;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo-section {
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
        }

        .logo-section img {
            width: 55px;
            height: 55px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid #4CAF50;
        }

        .logo-text {
            font-size: 20px;
            font-weight: 700;
            color: #1a1a1a;
            letter-spacing: 0.5px;
        }

        .nav-links {
            display: flex;
            gap: 35px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: #1a1a1a;
            font-size: 20px;
            font-weight: 700;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: #4CAF50;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: #4CAF50;
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Main content */
        .main-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: calc(100vh - 90px);
            padding: 40px 20px;
        }

        .cta-button {
            padding: 16px 50px;
            font-size: 22px;
            font-weight: 600;
            color: #4a4aff;
            background: #ffffff;
            border: 2px solid #8888cc;
            border-radius: 8px;
            cursor: pointer;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(74, 74, 255, 0.15);
            letter-spacing: 1px;
        }

        .cta-button:hover {
            background: #4a4aff;
            color: #ffffff;
            border-color: #4a4aff;
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(74, 74, 255, 0.3);
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 20px;
            color: #888;
            font-size: 14px;
        }
