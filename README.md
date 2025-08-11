Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Color Circles</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

<div class="circle-container">
    <div class="circle red">
        <div>
            <h3>Energy</h3>
            <p>Represents passion, excitement, and action.</p>
        </div>
    </div>
    <div class="circle blue">
        <div>
            <h3>Calm</h3>
            <p>Symbolizes peace, trust, and relaxation.</p>
        </div>
    </div>
    <div class="circle green">
        <div>
            <h3>Growth</h3>
            <p>Associated with nature, renewal, and balance.</p>
        </div>
    </div>
</div>

</body>
</html>
Css
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
}

.circle-container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    min-height: 100vh;
    flex-wrap: wrap;
}

.circle {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    padding: 20px;
    border: 5px solid white;
    box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    color: white;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: transform 0.3s ease;
}

.circle:hover {
    transform: scale(1.1);
}

.circle h3 {
    margin: 0 0 8px;
    font-size: 1.1em;
}

.circle p {
    margin: 0;
    font-size: 0.85em;
}

.red {
    background-color: #e63946;
}

.blue {
    background-color: #457b9d;
}

.green {
    background-color: #2a9d8f;
}
