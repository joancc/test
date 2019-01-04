<template>
  <div>Getting Data from axios</div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      items: []
    };
  },
  mounted() {
    axios
      .post("https://api-test.gestionix.com/api/v3/users/authentication", {
        user: "hogar@gestionix.com",
        password: "demo"
      })
      .then(function(response) {
        let accessKey = "Bearer " + response.data.access_token;
        let newUrl = "https://api-test.gestionix.com/api/v3/users/93";
        localStorage.setItem("access-token", accessKey);
        axios.defaults.headers.common["Authorization"] = localStorage.getItem(
          "access-token"
        );
        axios
          .get(newUrl)
          .then(function(res) {
            console.log(res.data);
          })
          .catch(function(err) {
            console.log(err);
          });
      })
      .catch(function(error) {
        console.log(error);
      });
  }
};
</script>