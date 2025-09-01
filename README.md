<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kodi im</title>

  <!-- 1️⃣ Shtojmë CSS të highlight.js (në <head>) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/atom-one-dark.min.css">

  <!-- CSS jonë personale -->
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #20232a;
      color: white;
      padding: 20px;
    }
    .code-block {
      margin: 20px 0;
      border-radius: 8px;
      overflow-x: auto;
    }
  </style>
</head>
<body>
  <!-- 2️⃣ Kodi që duam ta theksojmë -->
  <pre><code class="language-javascript">
function MyButton() {
  return (
    &lt;button&gt;I'm a button&lt;/button&gt;
  );
}
  </code></pre>

  <!-- 3️⃣ JavaScript i highlight.js (vendoset përpara </body>) -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
  <script>
    hljs.highlightAll(); // aktivizon highlight për çdo <pre><code>
  </script>
</body>
</html>
