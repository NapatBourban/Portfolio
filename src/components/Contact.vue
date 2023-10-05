<script>
import emailjs from "@emailjs/browser";

export default {
  data() {
    return {
      sendername: "",
      subject: "",
      message: "",
      replyto: "",
    };
  },
  methods: {
    sendMail() {
      emailjs.init("6cjSlOpO4U8I1wvxy");

      const params = {
        sendername: this.sendername,
        to: this.to,
        subject: this.subject,
        message: this.message,
        replyto: this.replyto,
      };
      const serviceID = "service_g0l7ovk";
      const templateID = "template_p08iqow";

      emailjs
        .send(serviceID, templateID, params)
        .then((res) => {
          alert("Email Sent");
        })
        .catch((error) => {
          console.error("Email send error:", error);
          alert("Error sending email. Please try again later.");
        });
    },
  },
};
</script>
<template>
  <div class="">
  
    <div class="container">
      <div class="d-flex justify-content-center"><p style="font-size: 95px;font-weight: 800;color:aliceblue;text-shadow: 10px 0px 0px black;">C</p><div
                class="colorchange mx-2"
                style="width: 60px; height: 60px; border-radius: 80%; margin-top: 4.2%;box-shadow: 10px 0px 0px black;"
              ></div> <p style="font-size: 95px;font-weight: 800;color:aliceblue;text-shadow: 10px 0px 0px black;" >ntact</p></div>
      <div class="d-flex justify-content-center">
        <form style="margin-top: 30px; margin-right: 0%; width: 500px; height: 570px">
          <div class="d-flex justify-content-center"><h3>Sent to Email</h3></div>
          <input
            type="text"
            class="border border-2 border-white"
            id="sendername"
            placeholder="yourname"
            v-model="sendername"
            required
          />
          <input
            type="email"
            class="border border-2 border-white"
            id="to"
            placeholder="to : Email@gmail.com"
            v-model="to"
            required
          />
          <input
            type="text"
            class="border border-2 border-white"
            id="subject"
            placeholder="subject"
            v-model="subject"
            required
          />
          <textarea
            type="text"
            class="border border-2 border-white"
            id="message"
            placeholder="message"
            v-model="message"
            required
          />
          <button
            type="button"
            class="btn btn-primary"
            data-bs-toggle="modal"
            data-bs-target="#exampleModal"
            v-on:click="sendMail()"
          >
            Send Email
          </button>
        </form>
        <div
          class="d-flex mx-5"
          style="width: 500px; height: 400px; margin-top: 80px; marign-left: 500px"
        >
          <div>
            <div class="box border border-2 border-wihte">
              <div class="d-flex mx-4 mt-3">
                <div
                  class="d-flex justify-content-center bg-black"
                  style="width: 80px; height: 70px; align-items: center;border-radius: 15px;"
                >
                  <img
                    src="../assets/envelope(1).png"
                    style="height: 30px; width: 30px; color: aliceblue"
                  />
                </div>
                <div class="mx-3">
                  <div class="headtext">Email Address</div>
                  <div class="bodytext">napatone123@gmail.com</div>
                </div>
              </div>
            </div>
            <div class="box border border-2 border-wihte">
              <div class="d-flex mx-4 mt-3">
                <div
                  class="d-flex justify-content-center bg-black"
                  style="width: 80px; height: 70px; align-items: center;border-radius: 15px;"
                >
                  <img
                    src="../assets/whatsapp(1).png"
                    style="height: 30px; width: 30px; color: aliceblue"
                  />
                </div>
                <div class="mx-3">
                  <div class="headtext">Phone No.</div>
                  <div class="bodytext">(+66) 61-368-1228</div>
                </div>
              </div>
            </div>
            <div class="box border border-2 border-wihte">
              <div class="d-flex mx-4 mt-3">
                <div
                  class="d-flex justify-content-center bg-black"
                  style="width: 80px; height: 70px; align-items: center;border-radius: 15px;"
                >
                  <img
                    src="../assets/facebook(1).png"
                    style="height: 30px; width: 30px; color: aliceblue"
                  />
                </div>
                <div class="mx-3">
                  <div class="headtext">Fackbook</div>
                  <div class="bodytext">ณภัทร บัวบาน</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
form {
  background-color: rgba(135, 130, 130, 0.5);
  display: flex;
  flex-direction: column;
  margin: 20px 50px 50px;
  width: 90%;
  max-width: 600px;
  border-radius: 10px;
}
form h3 {
  color: black;
  font-weight: 800;
  margin-bottom: 20px;
}
form input {
  border: 0px;
  margin: 10px 0;
  padding: 20px;
  background-color: rgba(135, 130, 130, 0.5);
  border-radius: 50px;
  margin: 20px 50px 0px;
  font-size: 18px;
  font-color: black;
}
form button {
  padding: 15px;
  background-color: #ff5351;
  font-size: 18px;
  border: none;
  cursor: pointer;
  width: 150px;
  margin: 20px auto 0;
  border-radius: 30px;
}
input {
  height: 60px;
}
textarea {
  height: 150px;
  margin: 20px 50px 0px;
  background-color: rgba(135, 130, 130, 0.5);
  border-radius: 15px;
}
::placeholder {
  color: rgb(255, 255, 255);
  opacity: 1;
}
.box {
  margin: 0px 0px 40px;
  width: 370px;
  height: 120px;
  border-radius: 20px;
}
.headtext {
  font-size: 20px;
  font-weight: 800;
  color: aliceblue;
}
.bodytext {
  font-size: 16px;
  font-weight: 500;
  color: rgb(148, 147, 147);
}
</style>
