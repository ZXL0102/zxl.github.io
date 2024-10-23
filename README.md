<h1 align="center">Welcome to my world</h1>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Four Horizontal Columns Layout</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            display: flex;
            flex-direction: row; /* 横向排列 */
            justify-content: space-between;
            padding: 20px;
            flex-wrap: wrap; /* 允许换行 */
        }
        .column {
            background-color: white;
            border: 1px solid #ccc;
            border-radius: 5px;
            padding: 15px;
            margin: 10px;
            flex: 1 1 calc(24% - 20px); /* 4 columns */
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        @media (max-width: 768px) {
            .column {
                flex: 1 1 calc(48% - 20px); /* 2 columns on smaller screens */
            }
        }
        @media (max-width: 480px) {
            .column {
                flex: 1 1 100%; /* 1 column on very small screens */
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="column">Column 1</div>
        <div class="column">Column 2</div>
        <div class="column">Column 3</div>
        <div class="column">Column 4</div>
    </div>
</body>
</html>
