# loginpage
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Login Page</title>
    <style>
        /* Basic reset and centering */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        /* Login container styling */
        .login-container {
            background-color: #ffffff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 300px;
        }

        .login-container h2 {
            margin-bottom: 20px;
            text-align: center;
            color: #333333;
        }

        /* Input group styling */
        .input-group {
            margin-bottom: 15px;
        }

        .input-group label {
            display: block;
            margin-bottom: 5px;
            color: #666666;
            font-size: 14px;
        }

        .input-group input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
        }

        .input-group input:focus {
            border-color: #007bff;
            outline: none;
        }

        /* Submit button styling */
        .login-btn {
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            border: none;
            border-radius: 4px;
            color: white;
            font-size: 16px;
            cursor: pointer;
            margin-top: 10px;
        }

        .login-btn:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

    <div class="login-container">
        <h2>Login</h2>
        <!-- Replace "action" attribute with your backend submission URL -->
        <form action="/login-endpoint" method="POST">
            
            <!-- Username/Email Field -->
            <div class="input-group">
                <label for="username">Username or Email</label>
                <input type="text" id="username" name="username" placeholder="Enter username" required>
            </div>
            
            <!-- Password Field -->
            <div class="input-group">
                <label for="password">Password</label>
                <input type="password" id="password" name="password" placeholder="Enter password" required>
            </div>
            
            <!-- Submit Button -->
            <button type="submit" class="login-btn">Log In</button>
            
        </form>
    </div>

</body>
</html>
