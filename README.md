<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login / Signup</title>
  <link rel="stylesheet" href="style.css">
  <link href="https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css" rel="stylesheet">
</head>
<body>
  <div class="container">
    <div class="form-box register">
      <h2 class="title animation" style="--i:17;--j:0">Sign Up</h2>
      <form action="#">
        <div class="input-box animation" style="--i:18;--j:1">
          <input type="text" required>
          <label>Username</label>
          <i class="bx bxs-user"></i>
        </div>
        <div class="input-box animation" style="--i:19;--j:2">
          <input type="email" required>
          <label>Email</label>
          <i class="bx bxs-envelope"></i>
        </div>
        <div class="input-box animation" style="--i:20;--j:3">
          <input type="password" required>
          <label>Password</label>
          <i class="bx bxs-lock-alt"></i>
        </div>
        <button type="submit" class="btn animation" style="--i:21;--j:4">Sign Up</button>
      </form>
    </div>
  </div>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(120deg, #6a11cb, #2575fc);
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  background: #fff;
  padding: 40px;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
  width: 350px;
}

.title {
  text-align: center;
  margin-bottom: 20px;
  font-size: 24px;
  color: #333;
}

.input-box {
  position: relative;
  margin: 20px 0;
}

.input-box input {
  width: 100%;
  padding: 10px 40px 10px 10px;
  border: 1px solid #ccc;
  border-radius: 8px;
}

.input-box label {
  position: absolute;
  top: 50%;
  left: 10px;
  transform: translateY(-50%);
  font-size: 14px;
  color: #aaa;
  pointer-events: none;
  transition: 0.3s;
}

.input-box input:focus ~ label,
.input-box input:valid ~ label {
  top: -8px;
  left: 10px;
  background: #fff;
  padding: 0 5px;
  color: #333;
  font-size: 12px;
}

.input-box i {
  position: absolute;
  right: 10px;
  top: 50%;
  transform: translateY(-50%);
  color: #666;
}

.btn {
  width: 100%;
  padding: 10px;
  background: #6a11cb;
  border: none;
  color: #fff;
  font-size: 16px;
  border-radius: 8px;
  cursor: pointer;
  transition: 0.3s;
}

.btn:hover {
  background: #2575fc;
}
