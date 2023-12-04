<!DOCTYPE html>
<html>
<head>
  <title>My Gallery</title>
  <style>
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
    }

    .gallery-item {
      flex: 1 0 200px;
      margin: 10px;
      text-align: center;
    }

    .gallery-item img {
      width: 100%;
      height: auto;
    }
  </style>
</head>
<body>
  <h1>My Gallery</h1>
  <div class="gallery">
    <div class="gallery-item">
      <img src="img/1.jpg" alt="Image 1">
    </div>
    <div class="gallery-item">
      <img src="img/2.jpg" alt="Image 2">
    </div>
    <div class="gallery-item">
      <img src="img/3.jpg" alt="Image 3">
    </div>
    <!-- Добавьте еще картинок, если необходимо -->
  </div>
</body>
</html>
