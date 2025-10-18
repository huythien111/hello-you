hello-you
20/10
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>chúc 20/10 vui vẻ</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
      background-color: #fff0f5;
    }

    h1 {
      color: #e91e63;
    }

    .buttons {
      margin-top: 40px;
      display: flex;
      justify-content: center;
      gap: 100px; /* khoảng cách giữa nút Có và Không */
    }

    button {
      padding: 15px 30px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .yes {
      background-color: #4CAF50;
      color: white;
    }

    .no {
      background-color: #f44336;
      color: white;
    }

    .image-container {
      margin-top: 40px;
      display: none;
    }

    .image-container img {
      max-width: 300px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }

    .message {
      margin-top: 20px;
      font-size: 20px;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>m hãy chọn 1 trong 2</h1>

  <div class="buttons">
    <button class="yes" onclick="showImage('yes')">trái</button>
    <button class="no" onclick="showImage('no')">phải</button>
  </div>

  <div class="image-container" id="imageBox">
    <img id="giftImage" src="" alt="Ảnh quà">
    <div class="message" id="messageText"></div>
  </div>

  <script>
    function showImage(choice) {
      const imageBox = document.getElementById("imageBox");
      const giftImage = document.getElementById("giftImage");
      const messageText = document.getElementById("messageText");

      imageBox.style.display = "block";

      if (choice === 'yes') {
        giftImage.src = "https://imgur.com/gallery/need-this-VYptNUe#/t/bouquet"; // ảnh quà
        messageText.textContent = "chúc mừng vào ô 10 bông hoa 🎁";
      } else {
        giftImage.src = "https://imgur.com/gallery/i-like-cats-Ck2CStP#/t/catmemes"; // ảnh meme
        messageText.textContent = "quà giống trái và t thích m";
      }
    }
  </script>
</body>
</html>
