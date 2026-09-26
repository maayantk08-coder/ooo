<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign In / Sign Up</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #000;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        .container {
            width: 680px;
            height: 450px;
            background: white;
            display: flex;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.4);
        }

        /* LEFT SIDE */
        .login-section {
            width: 50%;
            background: #fff;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 30px;
        }

        .login-section h1 {
            font-size: 28px;
            margin-bottom: 25px;
            color: #111;
        }

        .social {
            display: flex;
            gap: 15px;
            margin-bottom: 12px;
        }

        .social span {
            width: 32px;
            height: 32px;
            border: 1px solid #ddd;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: bold;
            color: #345;
            font-size: 14px;
        }

        .or {
            color: #777;
            font-size: 12px;
            margin-bottom: 8px;
        }

        .input-box {
            width: 240px;
            height: 38px;
            background: #e9edf2;
            border: none;
            padding: 0 12px;
            margin: 5px 0;
            outline: none;
            font-size: 12px;
        }

        .forgot {
            font-size: 13px;
            color: #555;
            margin: 15px 0;
        }

        .signin-btn {
            width: 122px;
            height: 36px;
            border: none;
            border-radius: 20px;
            background: linear-gradient(90deg, #ff5722, #ff2d2d);
            color: white;
            font-size: 11px;
            font-weight: bold;
            cursor: pointer;
        }

        /* RIGHT SIDE */
        .signup-section {
            width: 50%;
            background: linear-gradient(135deg, #ff3d32, #ff2828);
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;
        }

        .signup-section h1 {
            font-size: 28px;
            margin-bottom: 15px;
        }

        .signup-section p {
            font-size: 13px;
            line-height: 20px;
            margin-bottom: 25px;
            color: #ffeaea;
        }

        .signup-btn {
            width: 128px;
            height: 36px;
            border-radius: 20px;
            border: 1px solid white;
            background: transparent;
            color: white;
            font-size: 11px;
            font-weight: bold;
            cursor: pointer;
        }

        .signin-btn:hover,
        .signup-btn:hover {
            transform: scale(1.05);
        }

        /* MOBILE */
        @media (max-width: 700px) {
            .container {
                width: 95%;
                height: auto;
                flex-direction: column;
            }

            .login-section,
            .signup-section {
                width: 100%;
                min-height: 400px;
            }
        }
    </style>
</head>

<body>

    <div class="container">

        <!-- SIGN IN -->
        <div class="login-section">

            <h1>Sign in</h1>

            <div class="social">
                <span>f</span>
                <span>G+</span>
                <span>in</span>
            </div>

            <div class="or">
                or use your account
            </div>

            <input 
                type="email" 
                class="input-box" 
                placeholder="Email"
            >

            <input 
                type="password" 
                class="input-box" 
                placeholder="Password"
            >

            <div class="forgot">
                Forgot your password?
            </div>

            <button class="signin-btn">
                SIGN IN
            </button>

        </div>


        <!-- SIGN UP -->
        <div class="signup-section">

            <h1>Hello, Friend!</h1>

            <p>
                Enter your personal details and start<br>
                journey with us
            </p>

            <button class="signup-btn">
                SIGN UP
            </button>

        </div>

    </div>

</body>
</html>
