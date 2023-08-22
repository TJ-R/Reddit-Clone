<script>
import {defineComponent} from 'vue'

export default defineComponent({
  name: "Navbar.vue"
})
</script>

<template>
  <div id="top-nav">
    <img src="" alt="Reddit Logo"/>
    <input type="text" id="searchText" name="searchText" placeholder="Search Reddit">
    <div id="nav-btn-container">
      <button id="get-app-btn">Get App</button>
      <button id="login-btn">Log In</button>
      <div id="account-dropdown"></div>
    </div>
  </div>
  <div id="side-nav">

  </div>
</template>

<style scoped>
  ::-webkit-input-placeholder {
    color: grey;
  }
  :-moz-placeholder { /* Upto Firefox 18, Deprecated in Firefox 19  */
    color: grey;
  }
  ::-moz-placeholder {  /* Firefox 19+ */
    color: grey;
  }
  :-ms-input-placeholder {
    color: grey;
  }

  #top-nav {
    padding: 1rem 2rem;
    display: flex;
    justify-content: space-between;
    height: 7vh;
    width: 100%
  }

  #searchText {
    width: 400px;
    border: 1px solid dimgrey;
    border-radius: 15px;
    background-color: #282828;
    padding: 10px;
    color: dimgrey;
  }

  #get-app-btn {
    border-radius: 15px;
  }

  #login-btn {
    border-radius: 15px;
    background-color: orangered;
  }
</style>