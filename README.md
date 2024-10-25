# Web-images
Creting an image generating web
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Image Display Example</title>
</head>
<body>
  <h1>Static Image Display</h1>
  <img src="https://via.placeholder.com/300" alt="Sample Image" width="300">

  <h1>Dynamic Image Display</h1>
  <button onclick="generateImage()">Generate Image</button>
  <div id="image-container"></div>

  <script>
    function generateImage() {
      const img = document.createElement("img");
      img.src = "https://via.placeholder.com/300";
      img.alt = "Dynamically Generated Image";
      img.width = 300;
      
      const container = document.getElementById("image-container");
      container.innerHTML = ""; // Clear previous images
      container.appendChild(img);
    }
  </script>
</body>
</html>
