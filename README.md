# makiemka.github.io
<div class="gallery">
  <div class="gallery-item">
    <img src="img/1.jpg" alt="текст_альтернативного_описания">
  </div>
  <div class="gallery-item">
    <img src="img/2.jpg" alt="текст_альтернативного_описания">
  </div>
  <div class="gallery-item">
    <img src="img/3.jpg" alt="текст_альтернативного_описания">
  </div>
  <!-- Добавьте еще картинок, если необходимо -->
</div>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script>
$(document).ready(function() {
  $('.gallery-item').click(function() {
    var imgSrc = $(this).find('img').attr('src');
    var imgAlt = $(this).find('img').attr('alt');
    var imgTitle = $(this).find('img').attr('title');
    var imgDesc = $(this).find('img').attr('description');

    $('#lightbox').fadeIn();
    $('#lightbox img').attr('src', imgSrc);
    $('#lightbox .caption').html('<h2>' + imgTitle + '</h2><p>' + imgDesc + '</p>');
  });

  $('#lightbox').click(function() {
    $(this).fadeOut();
  });
});
</script>

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

#lightbox {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  z-index: 9999;
}

#lightbox img {
  max-width: 90%;
  max-height: 90%;
  margin: 0 auto;
  display: block;
}

#lightbox .caption {
  text-align: center;
  color: #fff;
  margin-top: 10px;
}
</style>
