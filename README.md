<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>DHMIS Themed Site</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div id="monitor">
    <div class="screen">
      <a href="about.html" class="character red"></a>
      <a href="blog.html" class="character yellow"></a>
      <a href="extra.html" class="character duck"></a>
    </div>
    <div class="face">
      <div class="eye left"></div>
      <div class="teeth"></div>
      <div class="eye right"></div>
    </div>
  </div>
</body>
</html>

body {
  margin: 0;
  background-color: #004c49;
  font-family: monospace;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

#monitor {
  width: 700px;
  height: 500px;
  background-color: #f5e3d4;
  border-radius: 40px;
  border: 10px solid #b8a69b;
  position: relative;
  padding: 20px;
  box-shadow: inset 0 0 40px #d2c1af;
}

.screen {
  background-color: #1d1d1d;
  width: 100%;
  height: 65%;
  border: 5px solid #222;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background-image: linear-gradient(#1d1d1d 1px, transparent 1px), linear-gradient(90deg, #1d1d1d 1px, transparent 1px);
  background-size: 40px 40px;
  position: relative;
}

.character {
  width: 80px;
  height: 80px;
  background-size: cover;
  transition: transform 0.2s ease;
}

.character:hover {
  transform: scale(1.2);
}

.red {
  background-image: url('https://i.imgur.com/YOUR_RED_GUY_IMAGE.png');
}

.yellow {
  background-image: url('https://i.imgur.com/YOUR_YELLOW_GUY_IMAGE.png');
}

.duck {
  background-image: url('https://i.imgur.com/YOUR_DUCK_IMAGE.png');
}

.face {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 40px;
  margin-top: 10px;
}

.eye {
  width: 40px;
  height: 40px;
  background-color: #000;
  border-radius: 50%;
}

.teeth {
  width: 200px;
  height: 40px;
  background: repeating-linear-gradient(
    to right,
    white 0 20px,
    #ccc 20px 22px
  );
  border: 3px solid #aaa;
  border-radius: 5px;
}


