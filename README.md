<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sogeon Hub</title>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #050505;
  color: white;
  overflow-x: hidden;
}

button {
  cursor: pointer;
  border: 0;
  border-radius: 10px;
  padding: 12px 18px;
  font-weight: bold;
}

/* LOGIN */

#loginScreen {
  position: fixed;
  inset: 0;
  background: #050505;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 9999;
}

.loginBox {
  width: min(90%, 430px);
  background: #111;
  padding: 35px;
  border-radius: 22px;
  text-align: center;
  box-shadow: 0 0 40px #000;
}

.loginBox h1 {
  font-size: 42px;
}

.google {
  width: 100%;
  background: white;
  color: black;
  margin-top: 10px;
}

.apple {
  width: 100%;
  background: #222;
  color: white;
  margin-top: 10px;
}

.demo {
  margin-top: 15px;
  background: #6c5ce7;
  color: white;
  width: 100%;
}

/* HEADER */

header {
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 20px;
  background: #0d0d0d;
  border-bottom: 1px solid #222;
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  font-size: 22px;
  font-weight: bold;
}

.coins {
  display: flex;
  gap: 10px;
}

.coinBox {
  background: #181818;
  padding: 8px 12px;
  border-radius: 10px;
}

/* PIGEON */

.pigeonScene {
  height: 180px;
  position: relative;
  overflow: hidden;
  background: linear-gradient(#090909, #111);

 
