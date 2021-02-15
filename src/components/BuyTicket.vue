<template>
  <div class="wrapper">
    <form @submit.prevent="handleSubmit">
      <label>First Name</label>
      <input type="text" v-model="firstName" required />
      <label>Last Name</label>
      <input type="text" v-model="lastName" required />
      <label>City</label>
      <select v-model="city">
        <option value="oslo">Oslo - 24.06.2021</option>
        <option value="london">London - 29.06.2021</option>
        <option value="miami">Miami - 08.07.2021</option>
        <option value="tel-aviv">Tel Aviv - 24.07.2021</option>
      </select>
      <button>Complete Order</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: "",
      lastName: "",
      city: "",
    };
  },
  methods: {
    handleSubmit() {
      let ticketDetails = {
        firstName: this.firstName,
        lastName: this.lastName,
        city: this.city,
      };
      // Mangeler funksjon for å lukke modal på sumbit
      console.log(ticketDetails);
    },
  },
};
</script>

<style>
form {
  padding: 20px;
  border-radius: 10px;
}
label {
  display: block;
  text-align: left;
  color: #f3f3f3;
  text-transform: uppercase;
  font-size: 14px;
  font-weight: bold;
  margin: 20px 0 10px 0;
}
input,
select {
  border: 1px solid #ddd;
  padding: 10px;
  width: 100%;
  box-sizing: border-box;
}

select {
  margin-bottom: 40px;
}

form button {
  background: #394453;
  border: 2px solid #f3f3f3;
  padding: 12px 22px;
  font-size: 18px;
}
</style>