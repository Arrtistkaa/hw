
<!DOCTYPE HTML>
<html>

<body>
  
<h1>HTML Получить координаты геолокации</h1>

<button onclick="getLocation()">Попробовать</button>

<p id="demo"></p>

<script>
var x = document.getElementById("demo");

function getLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(showPosition);
    } else { 
        x.innerHTML = "Браузер не поддерживает геолокацию.";
    }
}

function showPosition(position) {
    x.innerHTML = "Широта: " + position.coords.latitude + 
    "<br>Долгота: " + position.coords.longitude;
}
</script>
  <hr>
  <svg width="100" height="100">
  <circle cx="50" cy="50" r="40"
  stroke="green" stroke-width="4" fill="yellow" />
Извините, Ваш браузер не поддерживает встроенный SVG.
</svg>
  <h1>вот так заголовок!</h1>
  <hr>
  <p>Текст.</p>
  <p>Изображение:</p>
  <img src=".jpg" width="200" height="200">
  <hr>
  <p>normal</p>
  <p style="color:red;">red</p>
  <p style="color:blue;">blue</p>
  <p style="font-size:67px;">big</p>
  <p style="text-align:center;">Параграф по центру.</p>
  <p>Это <sub>подстрочный</sub> текст.</p>
  <p>Это <sup>надстрочный</sup> текст.</p>
  <p>Мой любимый цвет <del>синий</del> <ins>красный</ins>.</p>
  <img src=".jpg" width="220" height="277" alt="The Scream">
  <p><cite>Крик</cite> Эдвард Мунк. Написана в 1893.</p>
  <!-- Это комментарий -->
  <h2 style="color:blue;">Это заголовок синий</h2>
  <img src="pic_mountain.jpg" alt="Вид на горы" style="width:304px;height:228px;">
  
  <title>JavaScript в script | Редактор HTML | schoolsw3.com</title>
  <script>
  function myFunction() {
    document.getElementById("demo").innerHTML = "Привет JavaScript!";
  }
  </script>
  <form action="/action_page.php" autocomplete="on">
  <label for="fname">Имя:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Фамилия:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Отправить">
</form>
  <h2>Форма с вводом кнопки radio</h2>
<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  Ваш браузер не поддерживает HTML5 видео.
</video>
<form>
  <input type="radio" name="gender" value="male" checked> Мужчина<br>
  <input type="radio" name="gender" value="female"> Женщина<br>
  <input type="radio" name="gender" value="other"> другое
  <form>
  <label for="birthday">День рождения:</label>
  <input type="date" id="birthday" name="birthday">
</form>
<form action="/action_page.php">
  Веб Страница: <input type="url" list="url_list" name="link">
  <datalist id="url_list">
    <option label="SchoolsW3" value="https://schoolsw3.com">
    <option label="Google" value="http://www.google.com">
    <option label="Microsoft" value="http://www.microsoft.com">
  </datalist>
  <input type="submit">
</form>
</body>

</html>
