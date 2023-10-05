<script setup>
import AboutMe from "../components/AboutMe.vue";
import Education from "../components/Education.vue";
import Cetificate from "../components/Certificate.vue";
import Contact from "../components/Contact.vue";
import Tab from "../components/Tab.vue";
import Skill from "../components/Skill.vue";
import portfolio from "../components/Portfolio.vue";
</script>

<template>
  <main>
    <div>
      <div class="w-100 bg-blue-100 d-flex div " style="height: 750px;background-color:rgba(50,49,55)" id="Profile">
        <div class="w-50 " style="margin-top: 15%;margin-left: 15%;">
          <h1 class="w-100" style="font-weight: 1000;color:#D1D1D1">I'M</h1>
          <div class="text-box" ><h1>NAPAT</h1></div>
          <span style="font-size: 40px;font-weight: 1000;color:#9B9B9B">Programer</span>
          <div class="mt-3 border border-2" style="height: 45px;width:120px;border-radius: 15px;"><a class="d-flex justify-content-center"  style="font-weight: 800;color:#FFFF;text-align: center;font-size: 20px;" href="https://drive.google.com/file/d/15bwlpb3dvMWSqyQi9jta6kO9Gs7fLJXE/view?usp=sharing">Resume</a></div>
        </div>
        <div class="w-50 d-flex justify-content-start mt-5">
          <div class="position-absolute">
              <img
                src="../assets/LINEALBUM2023.9.27230933.png "
                style="
                  width: 350px;
                  height: fit-content;
                  margin: 20px;
                  text-shadow: white 0.1em 0.1em 0.2em;
                "
                
              />
      </div>
    
        </div>
      </div>
      <div id="AboutMe" style="background-color:#9B9B9B ;height:650px" >
        <AboutMe></AboutMe>
      </div>
      <div style="background-color:rgba(50,49,55);height:450px">
        <Education></Education>
      </div>
      <div style="background-color: #9B9B9B;height:850px">
        <Skill></Skill>
      </div>
      <div id="Mywork" style="background-color: rgba(50,49,55);height:1100px">
        <portfolio></portfolio>
      </div>
      <div style="background-color: #9B9B9B;height:1150px"> 
        <Cetificate></Cetificate>
      </div>
      <div id="Contact"  style="background-color: rgba(50,49,55);height:800px">
        <Contact></Contact>
      </div>
      <div class="d-flex w-100 justify-content-center " style="background-color: #9B9B9B"> 
      <a href="#Profile" class="fonttab mt-2 mb-3">Profile</a>
      <a href="#AboutMe" class="mx-5 fonttab mt-2">About Me</a>
      <a class="fonttab mt-2 mb-3 me-5" href="#Mywork" >My Work</a>
      <a href="#Contact" class="fonttab mt-2">Contact</a>
      </div>
    </div>
  </main>
</template>
<style scoped> 
.textname {
  color: #ffff00;
}
.box {
  position: relative;
  width: 300px;
  height: 400px;
  background-color: rgb(246, 255, 0);
  margin-top: 100px;
  border-radius: 20%;
}
.text-box h1{
  font-size: 120px;
  margin-left: -10px;
  line-height: 100px;
  color:transparent;
  -webkit-text-stroke: 1px #ffff;
  background: url("../assets/back.png");
  -webkit-background-clip: text;
  background-position: 0 0;
  animation: back 20s linear infinite;

}
@keyframes back{
  100%{
    background-position: 2000px 0;
  }
}
.fonttab{
  font-size: 18px;
  font-weight: 800;
  color:rgb(246, 226, 203);

}

</style>
