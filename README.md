
<html>
<head>
    <title>User Profile</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            width: 400px;
        }
        h2 {
            text-align: center;
        }
        label {
            font-weight: bold;
        }
        input, textarea {
            width: 100%;
            padding: 8px;
            margin: 5px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        input[readonly] {
            background-color: #e9e9e9;
        }
        input[type="submit"] {
            background-color: #28a745;
            color: white;
            border: none;
            cursor: pointer;
            padding: 10px;
            font-size: 16px;
        }
        input[type="submit"]:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>User Profile</h2>
        <form action="profile_update.php" method="post">
            <label for="fullname">Full Name:</label>
            <input type="text" id="fullname" name="fullname" value="Name and Surname" readonly>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" value="Name@example.com" readonly>
            
            <label for="phone">Phone Number:</label>
            <input type="tel" id="phone" name="phone" value="456-123-7897">
            
            <label for="address">Address:</label>
            <textarea id="address" name="address" rows="3">123 Main Street, City, Country</textarea>
            
            <label for="bio">Bio:</label>
            <textarea id="bio" name="bio" rows="3">A short description about the user.</textarea>
            
            <input type="submit" value="Update Profile">
        </form>
    </div>
</body>
</html>
