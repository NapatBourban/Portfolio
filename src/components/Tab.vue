<script>
export default { components: { router } };
import router from "../router";
</script>
<template>
  <header :class="{ 'scrolled-nav': scolleNav }">
    <div class="w-100">
      <nav class="navbar navbar-dark">
        <div class="d-flex w-100">
          <div class="mx-2">
            <div class="d-flex">
              <h3 class="text" style="font-weight: 1000; font-size: 28px">P</h3>
              <div
                class="colorchange"
                style="width: 15px; height: 15px; border-radius: 80%; margin-top: 12%"
              ></div>
              <h3 class="text" style="font-weight: 1000; font-size: 28px">rtf</h3>
              <div
                class="colorchange"
                style="width: 15px; height: 15px; border-radius: 80%; margin-top: 12%"
              ></div>
              <h3 class="text" style="font-weight: 1000; font-size: 28px">li</h3>
              <div
                class="colorchange"
                style="width: 15px; height: 15px; border-radius: 80%; margin-top: 12%"
              ></div>
            </div>
          </div>
          <div
            class="container-fluid d-flex justify-content-end"
            style="font-weight: 1000"
          >
            <a class="text me-3" href="#Profile" style="font-size: 18px">Profile</a>
            <a class="text me-3" href="#AboutMe" style="font-size: 18px">About Me</a>
            <a class="text me-4 " href="#Mywork" style="font-size: 18px">My Work</a>
            <div
              class="bg-info d-flex justify-content-center mx-3"
              style="
                width: 100px;
                height: 30px;
                transition: all 0.3s ease 0s;
                border-radius: 50px;
              "
            >
              <a class="text mx-5" href="#Contact" style="font-size: 18px">Contact</a>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>
<style>
header {
  background-color: rgba(12, 12, 12, 0.8);
  z-index: 99;
  width: 100%;
  position: fixed;
  transition: 0.5s ease all;

  nav {
    display: flex;
    flex-direction: row;
    padding: 12px 0;
    transition: 0.5s ease all;
    width: 90%;
    margin: 0 auto;
    @media (min-width: 1140px) {
      max-width: 1140px;
    }
  }
}
header:hover {
  background-color: rgb(254, 254, 254, 0.3);
}
header:hover a {
  color: black;
}
header:hover h3 {
  color: black;
}
.colorchange {
  background-color: rgb(254, 254, 254);
}

header:hover .colorchange {
  background-color: rgb(0, 0, 0);
}
.text {
  color: rgb(246, 245, 245);
}
</style>
