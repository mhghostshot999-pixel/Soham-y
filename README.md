<!DOCTYPE html><html lang="mr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Free Fire Tournament Registration</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f0f0;
      padding: 20px;
    }
    .container {
      max-width: 400px;
      margin: auto;
      background: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    button {
      width: 100%;
      padding: 10px;
      background: #2e86ff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Free Fire Tournament Registration</h2><form id="regForm">
  <label>नाव लिहा:</label>
  <input type="text" id="name" required />

  <label>मोबाइल नंबर:</label>
  <input type="tel" id="mobile" required />

  <button type="submit">Submit</button>
</form>

  </div>  <script>
    const form = document.getElementById("regForm");

    form.addEventListener("submit", function (e) {
      e.preventDefault();

      const name = document.getElementById("name").value;
      const mobile = document.getElementById("mobile").value;

      // WhatsApp number where message will be sent
      const adminNumber = "918624938382"; // Your provided number (with country code)

      const message = `Free Fire Registration\nनाव: ${name}\nमोबाईल: ${mobile}`;

      const url = `https://wa.me/${adminNumber}?text=${encodeURIComponent(message)}`;

      window.open(url, "_blank");
    });
  </script></body>
</html>
