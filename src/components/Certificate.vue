<script></script>
<template>
  <div class="d-flex justify-content-center">
    <h1
      style="font-size: 100px; color: aliceblue; text-shadow: 7px 0px 0px rgb(0, 0, 0,0.8)"
    >
      Catificate
    </h1>
  </div>
  <div class="container d-flex justify-content-center">
    <div class="card">
      <img src="../assets/17199.jpg" />
      <div class="intro">
        <h3>Depa</h3>
        <p class="me-2">2022 Received a certificate from Unity's AR VR knowledge test.</p>
      </div>
    </div>
    <div class="card">
      <img src="../assets/AR.png" />
      <div class="intro">
        <h3>AR VR MR</h3>
        <p>
          2022 Passed training in product development or design. and services with basic
          AR, VR, MR and 3D technology and innovation.
        </p>
      </div>
    </div>
  </div>
  <div class="container d-flex justify-content-center">
    <div class="card">
      <img src="../assets/catificate1.jpg" />
      <div class="intro">
        <h3>เหรียญเรียนดี ปี1</h3>
        <p>2022 Received a good academic medal with Grade : 3.69, University Year 1</p>
      </div>
    </div>
    <div class="card">
      <img src="../assets/catificate2.jpg" />
      <div class="intro">
        <h3>เหรียญเรียนดี ปี2</h3>
        <p>2023 Received a good academic medal with Grade : 3.69, University Year 2</p>
      </div>
    </div>
  </div>
</template>
<style scoped>
img {
  height: 400px;
  width: 600px;
  border-radius: 3px;
}
.container {
  display: flex;
}
.card {
  height: 400px;
  margin: 30px;
  box-shadow: 5px 5px 20px black;
  overflow: hidden;
}
.intro {
  height: 40px;
  width: 600px;
  padding: 6px;
  bottom: 0px;
  box-sizing: border-box;
  position: absolute;
  background-color: rgb(27, 27, 27, 0.5);
  color: white;
}
h1 {
  margin: 10px;
  font-size: 40px;
}
p {
  font-size: 15px;
  margin: 20px;
  visibility: hidden;
  opacity: 0;
}
.card:hover {
  cursor: pointer;
}
.card:hover .intro {
  height: 150px;
  bottom: 0px;
  background-color: black;
}
.card:hover p {
  opacity: 1;
  visibility: visible;
}
</style>
