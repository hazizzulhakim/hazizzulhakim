@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@400;500;600;700;800&family=Poppins:wght@400;500;600&display=swap");

* {
  margin: 0;
  padding: 0;
  font-family: "Nunito", sans-serif;
  font-weight: 500;
}
html {
  scroll-behavior: smooth;
}
body {
  text-align: center;
  max-width: 600px;
  position: relative;
  margin: auto;
  background: black;
}
.preload {
  position: fixed;
  z-index: 9999;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: black;
  display: flex;
  justify-content: center;
  align-items: center;
}

.preload p {
  color: #fff;
  animation: load 3s ease;
  -webkit-animation: load 1s ease infinite;
}

@keyframes load {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0.2;
  }
  100% {
    opacity: 1;
  }
}

.open {
  position: fixed;
  z-index: 10;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow-x: hidden;
  background-color: black;
  background-size: cover;
}
.open div {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.open div.lope {
  height: 70px;
  width: 70px;
  margin: 20px 0;
  margin-top: 60px;
  background: rgb(255, 255, 255);
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  border-radius: 50%;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  animation: anm 1s infinite ease;
  -webkit-animation: anm 1s infinite ease;
  box-shadow: 5px 5px 30px rgba(0, 0, 0, 0.2);
}

.open i {
  font-size: 2.3em;
  color: red;
}

.open h3 {
  font-weight: 500;
  color: white;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
}

#bg {
  background-image: linear-gradient(to top, rgba(0, 0, 0, 0.42), rgba(0, 0, 0, 0.511)), url("Foto1.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  top: 0;
  bottom: 0;
  width: 100vw;
  max-width: 600px;
  position: fixed;
  z-index: -1;
}

img#fotoku {
  max-width: 200px;
  margin: 50px auto 20px;
  opacity: 0;
  transform: translateY(30px) scale(0.3);
  -webkit-transform: translateY(30px) scale(0.3);
  -moz-transform: translateY(30px) scale(0.3);
  -ms-transform: translateY(30px) scale(0.3);
  -o-transform: translateY(30px) scale(0.3);
}

h2#hai,
h3#hia {
  font-weight: 500;
  color: white;
  text-shadow: 2px 2px 5px black;
}
h2#hai,
h3#hia {
  opacity: 0;
  transform: translateY(20px);
  -webkit-transform: translateY(20px);
  -moz-transform: translateY(20px);
  -ms-transform: translateY(20px);
  -o-transform: translateY(20px);
}
#slider {
  display: flex;
  overflow: scroll;
  overflow-y: hidden;
  width: 90%;
  margin: auto;
  height: fit-content;
  padding: 10px 0;
  flex-flow: row nowrap;
  scroll-snap-type: x mandatory;
  scrollbar-width: none;
  opacity: 0;
  transform: translateY(-20px) scale(0.5);
  -webkit-transform: translateY(-20px) scale(0.5);
  -moz-transform: translateY(-20px) scale(0.5);
  -ms-transform: translateY(-20px) scale(0.5);
  -o-transform: translateY(-20px) scale(0.5);
}
#slider::-webkit-scrollbar {
  display: none;
}
#slider p {
  font-size: 1.2em;
  color: white;
  text-shadow: 2px 2px black;
  font-weight: 500;
  text-align: center;
  scroll-snap-align: center;
  flex: none;
  width: 80%;
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 10px;
  padding: 10px 20px;
  box-sizing: border-box;
  background: rgba(0, 0, 0, 0.425);
  border: 2px dashed rgb(255, 255, 255);
  border-radius: 10px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
#slider p:first-child {
  margin-left: 10%;
}
#slider p:last-child {
  margin-right: 10%;
}
span {
  margin-left: 5px;
  cursor: pointer;
  animation: anm 1s infinite;
  -webkit-animation: anm 1s infinite;
}

@keyframes anm {
  0% {
    transform: scale(1);
    -webkit-transform: scale(1);
    -moz-transform: scale(1);
    -ms-transform: scale(1);
    -o-transform: scale(1);
  }
  50% {
    transform: scale(1.2);
    -webkit-transform: scale(1.2);
    -moz-transform: scale(1.2);
    -ms-transform: scale(1.2);
    -o-transform: scale(1.2);
  }
  100% {
    transform: scale(1);
    -webkit-transform: scale(1);
    -moz-transform: scale(1);
    -ms-transform: scale(1);
    -o-transform: scale(1);
  }
}
