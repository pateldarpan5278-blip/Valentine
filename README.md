<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
<title>Valentine 💘</title>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Rubik+Glitch&display=swap" rel="stylesheet">

<style>
:root {
  --pink: #ff4d6d;
  --purple: #7b2cbf;
  --red: #ff006e;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  height: 100vh;
  overflow: hidden;
  font-family: 'Pacifico', cursive;
  background: linear-gradient(135deg, #ff4d6d, #ff006e, #7b2cbf);
  background-size: 400% 400%;
  animation: bgMove 10s ease infinite;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
}

/* Background animation */
@keyframes bgMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* Floating hearts */
.heart {
  position: fixed;
  font-size: 20px;
  animation: floatUp linear infinite;
  opacity: 0.8;
}

@keyframes floatUp {
  from {
    transform: translateY(100vh) scale(0.6);
    opacity: 0;
  }
  to {
    transform: translateY(-10vh) scale(1.2);
    opacity: 1;
  }
}

/* Center content */
.container {
  text-align: center;
  padding: 20px;
  z-index: 10;
}

h1 {
  font-family: 'Rubik Glitch', cursive;
  font-size: clamp(2.2rem, 8vw, 3.5rem);
  text-shadow: 0 0 15px #fff, 0 0 30px var(--pink);
  animation: pulse 1.8s infinite;
}

@keyframes pulse {
  0%,100% { transform: scale(1); }
  50% { transform: scale(1.08); }
}

/* Buttons */
.buttons {
  margin-top: 30px;
  display: flex;
  gap: 20px;
  justify-content: center;
}

button {
  font-size: 1.3rem;
  padding: 15px 30px;
  border-radius: 50px;
  border: none;
  cursor: pointer;
  transition: transform 0.3s, box-shadow 0.3s;
}

#yesBtn {
  background: linear-gradient(45deg, #ff4d6d, #ff85a1);
  color: white;
  box-shadow: 0 0 15px #ff85a1;
}

#yesBtn:active {
  transform: scale(0.95);
}

#noBtn {
  background: #fff;
  color: #ff006e;
  position: relative;
}

/* Celebration */
.celebrate {
  display: none;
  position: fixed;
  inset: 0;
  background: radial-gradient(circle, rgba(255,255,255,0.15), transparent);
  z-index: 20;
  text-align: center;
  padding-top: 20vh;
}

.celebrate h2 {
  font-family: 'Rubik Glitch', cursive;
  font-size: clamp(2.5rem, 9vw, 4rem);
  color: #fff;
  text
