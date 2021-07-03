<template>
  <div class="contact-container">
    <div class="contact">
      <div>
        <h1 class="contact-title">Let's Talk</h1>
        <p>Email: pedroblimaa@gmail.com</p>
        <p class="contact-text">
          <a href="https://twitter.com/pedroblimaa2" target="_blank">
            Twitter</a
          >
        </p>
        <p class="contact-text">
          <a
            href="https://www.linkedin.com/in/pedro-bonfilio-lima-0693a914a/"
            target="_blank"
          >
            Linkedin
          </a>
        </p>
      </div>
      <div class="form-container">
        <h3 class="form-title">Or get in touch by the form below</h3>
        <div class="input-container">
          <p>Name:</p>
          <Input placeholder="Insert your name" />
        </div>
        <div class="input-container">
          <p>Email:</p>
          <Input placeholder="Insert your email" />
        </div>
        <div class="input-container">
          <p>Message:</p>
          <TextInput placeholder="Insert your message" />
        </div>
        <button v-on:click="sendHello">Clique aqui</button>
      </div>
    </div>
  </div>
</template>

<script>
import Input from "@/components/Input/Input";
import TextInput from "@/components/TextInput/TextInput";
// import api from "@/services/api.js";
import api from '@/services/api'

export default {
  name: "Contact",
  components: {
    Input,
    TextInput,
  },
  methods: {
    sendHello: async function () {
      api
        .post("/email", {
          name: 'Pedro',
          email: 'pedroblimaa@gmail.com',
          text: 'Esse é um texto!!'
        })
        .then((resp) => {
          let result = resp.data;
          console.log(result);
        })
        .catch((error) => {
          console.log(error);
        });
    },
  },
};
</script>

<style scoped src="./Contact.css">
</style>
