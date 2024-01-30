<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DARKPATTERN DETECTOR</title>
    <link rel="stylesheet" href="style.css">
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Google Search Bar</title>
        <style>
            body {
                font-family: 'Arial', sans-serif;
                background-color: #f0f0f0;
                margin: 0;
                padding: 0;
                display: flex;
                justify-content: center;
                align-items: center;
                height: 100vh;
            }
    
            #searchContainer {
                background-color: #4285f4; /* Google Blue Color */
                padding: 20px;
                border-radius: 10px;
                box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
                text-align: center;
            }
    
            #searchInput {
                width: 300px;
                padding: 10px;
                font-size: 16px;
                border: none;
                border-radius: 5px;
            }
    
            #searchButton {
                padding: 10px;
                font-size: 16px;
                cursor: pointer;
                background-color: #34a853; /* Google Green Color */
                color: #fff;
                border: none;
                border-radius: 5px;
            }
        </style>
    </head>
    <body>
        <div id="searchContainer">
            <input type="text" id="searchInput" placeholder="Google Search">
            <button id="searchButton">Google Search</button>
        </div>
    </body>
    </html>
    
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: transparent;
        }

        .main {
            text-align: center;
            margin-top: 50px;
        }

        .navbar {
            background-color: #333;
            color: white;
            padding: 10px;
        }

        .icon {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        #searchContainer {
            background-color: transparent;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(236, 129, 6, 0.1);
            margin-top: 20px;
        }

        #searchInput {
            width: 100%;
            padding: 8px;
            margin-bottom: 16px;
            box-sizing: border-box;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        #searchButton {
            padding: 8px;
            font-size: 16px;
            cursor: pointer;
        }

        #result {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="main">
        <div class="navbar">
            <div class="icon">
                <h2 class="logo">SAFESiTe</h2>
            </div>
            <div class="menu">
                <ul>
                    <li><a href="#">HOME</a></li>
                    <li><a href="#">SIGN.IN</a></li>
                    <li><a href="#">FEEDBACK</a></li>
                    <li><a href="#">SETTINGS</a></li>
                </ul>
            </div>
        </div>

        <div id="searchContainer">
            <input type="text" id="searchInput" placeholder="Enter URL...">
            <button id="searchButton" onclick="searchURL()">Search</button>
            <div id="result"></div>
        </div>
    </div>

    <script>
        function searchURL() {
            var input = document.getElementById('searchInput').value;
            var blockedTerms = ['fake', 'scam', 'hidden-cost', 'urgent'];

            for (var i = 0; i < blockedTerms.length; i++) {
                if (input.toLowerCase().includes(blockedTerms[i])) {
                    document.getElementById('result').innerHTML = 'Blocked URL. Please enter a valid URL.';
                    return;
                }
            }

            document.getElementById('result').innerHTML = 'Valid URL: ' + input;
        }
    </script>
</body>


</html>
