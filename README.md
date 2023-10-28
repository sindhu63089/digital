# digital
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Web Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        #container {
            padding: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #007BFF;
            color: #fff;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div id="container">
        <h1>Welcome to My Interactive Web Page</h1>
        <button id="colorChangeButton">Change Background Color</button>
    </div>
    <div>
        <h2>ABOUT ME</h2>
        <P>sindhu kamachi</P>
        <div>
            <h3>MY UNIVARCITY</h3>
            <P>BHARATHIYAR UNIVARCITY</P>
        </div>
        <div>
            <h4>MY COLLEGE</h4>
            <P>KARUPPANAN MARIAPPAN COLLEGE</P>
        </div>
        <div>
            <h5>Contact</h5>
            <p>+91 3526418797</p>
        </div>
        <div>
            <h6>gmail</h6>
            <p>www.sindhu@gmail.com</p>
        </div>
    <script>
        // JavaScript code to change the background color
        const button = document.getElementById("colorChangeButton");
        const colors = ["#007BFF", "#FF5722", "#27AE60", "#E91E63"];
        let currentColorIndex = 0;

        button.addEventListener("click", function () {
            document.body.style.backgroundColor = colors[currentColorIndex];
            currentColorIndex = (currentColorIndex + 1) % colors.length;
        });
    </script>
</body>
</html>
