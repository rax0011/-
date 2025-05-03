<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>اضحكي أوجي</title>
  <style>
    body { background-color: #fefefe; font-family: Arial; text-align: center; direction: rtl; padding: 50px; }
    h1 { color: #ff5e57; }
    .joke-box { background: #fff; padding: 20px; margin: auto; border-radius: 10px; box-shadow: 0 0 10px #ccc; max-width: 500px; }
    button { margin-top: 20px; padding: 10px 20px; background: #ff5e57; color: white; border: none; border-radius: 5px; cursor: pointer; }
  </style>
</head>
<body>
  <h1>اضحكي أوجي</h1>
  <div class="joke-box">
    <p id="joke">مره واحد راح للدكتور، قاله بطني توجعني، قاله الدكتور: من متى؟ قاله: من أمس، قاله روح وتعال بكره!</p>
    <button onclick="newJoke()">نكتة جديدة</button>
  </div>

  <script>
    const jokes = [
      "فيه واحد راح يشتري نظارة، قال للبائع: عندك نظارات للمستقبل؟",
      "مره مدرس رياضيات خلف ولد سماه: سالب.",
      "واحد غبي راح يسوي تحليل دم، طلع معه فصيلة ببسي.",
      "مره واحد لقوه ميت قدام الثلاجة، كاتب: مافي شي ناكله."
    ];

    function newJoke() {
      const joke = jokes[Math.floor(Math.random() * jokes.length)];
      document.getElementById('joke').textContent = joke;
    }
  </script>
</body>
</html>
