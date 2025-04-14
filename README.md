<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CMI Hotel 1935 Chat</title>
  <style>
    body { margin: 0; }
    #chat-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #2e7d32;
      color: white;
      border: none;
      border-radius: 50px;
      padding: 14px 24px;
      font-size: 16px;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      z-index: 9999;
    }
    #chat-box {
      display: none;
      position: fixed;
      bottom: 80px;
      right: 20px;
      width: 360px;
      height: 500px;
      border: 2px solid #ccc;
      border-radius: 10px;
      overflow: hidden;
      z-index: 9999;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    iframe {
      width: 100%;
      height: 100%;
      border: none;
    }
  </style>
</head>
<body>

<button id="chat-btn">Chat with us</button>

<div id="chat-box">
  <iframe src="https://vipenmehta.github.io/cmi-chat-widget/"></iframe>
</div>

<script>
  const btn = document.getElementById("chat-btn");
  const box = document.getElementById("chat-box");
  btn.onclick = () => {
    box.style.display = box.style.display === "none" ? "block" : "none";
  };
</script>

</body>
</html>
