<div class="gallery">
  <a target="_blank" href="img/1.jpg">
    <img src="img/1.jpg" alt="текст_альтернативного_описания">
  </a>
  <a target="_blank" href="img/2.jpg">
    <img src="img/2.jpg" alt="текст_альтернативного_описания">
  </a>
  <a target="_blank" href="img/3.jpg">
    <img src="img/3.jpg" alt="текст_альтернативного_описания">
  </a>
  <!-- Добавьте еще картинок, если необходимо -->
</div>

<style>
.gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.gallery a {
  flex: 1 0 200px;
  margin: 10px;
  text-align: center;
}

.gallery img {
  width: 100%;
  height: auto;
}
</style>
