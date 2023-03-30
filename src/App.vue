<template >
  <div>
    <section>      
      <form action="">
        <table>
          <tr>
            <td>Ten dang nhap</td>
            <td><input type="text" v-model="friend.name"></td>
          </tr>

          <tr>
            <td>Mat khau</td>
            <td><input type="password" v-model="friend.password"></td>
          </tr>
          <tr>
            <td></td>
            <td><button type="submit" @click="sendData">Dang nhap</button>
                <button type="reset" @click="clearData">Xoa</button>
            </td>
          </tr>
        </table>
      </form>
    <h3>
      {{ friend }}
    </h3>
    </section>
  </div>
</template>
<script>

import axios from 'axios';

export default {
  data() {
    return {
      friend: {
        name: "",
        password: ""
      }
    }
  },
  methods: {
    sendData(e) {
      e.preventDefault();
      console.log("senndData active !!!");

    axios.post("http://localhost:81/API/api.php", {
      name: this.friend.name,
      password: this.friend.password
        })
        .then(function (response) {
          console.log(response);
        })
        .catch(function (error) {
          console.log(error);
        });

      this.clearData();
    },
    clearData() {
      this.friend.name = "";
      this.friend.password = "";
    }
  }
}
</script>

<style>
  
</style>