<template>
  <div class="contact-form">
    <h2>Contact Us</h2>
    <form v-on:submit.prevent="greetUser">
      <input type="text" v-model="username" placeholder="Your Name" />
      <input type="email" v-model="useremail" placeholder="Your Email" />
      <textarea v-model="usermessage" placeholder="Your Message"></textarea>
      <button type="submit">Send Message</button>
    </form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      username: "",
      useremail: "",
      usermessage: ""
    };
  },
  methods: {
    greetUser() {
      alert(`Hello ${this.username}, your message has been sent successfully!`);
    }
  }
};
</script>
