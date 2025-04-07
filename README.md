<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>zlera</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
    }
    header {
      background-color: #222;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .container {
      max-width: 900px;
      margin: 30px auto;
      padding: 20px;
      background-color: white;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h2 {
      margin-top: 0;
    }
    textarea {
      width: 100%;
      height: 200px;
      margin-top: 10px;
      padding: 10px;
      font-family: monospace;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      margin-top: 10px;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 4px;
    }
    pre {
      background-color: #f4f4f4;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
      overflow-x: auto;
    }
  </style>
</head>
<body>
  <header>
    <h1>Code Share</h1>
    <p>Share your code snippets with the world</p>
  </header>

  <div class="container">
    <h2>share here</h2>
    <textarea id="codeInput" placeholder="Enter your code here..."></textarea>
    <button onclick="shareCode()">Share</button>

    <h2>Shared Code</h2>
    <pre id="sharedCode"></pre>
  </div>

  <script>
    function shareCode() {
      const code = document.getElementById('codeInput').value;
      document.getElementById('sharedCode').textContent = code;
    }
  </script>
</body>
</html>


