<script>
  import logo from "./icons/Logomark.png"
  import settings from "./icons/settings-icon.png"
  import bell from "./icons/Bell.png"
  import search from "./icons/search.png"
  import burger from "./icons/burger.png"
  import avatar from "../assets/images/Avatar.png"
  import Button from "./Button.vue"

  export default {
    name: "Navbar",
    
    data: function () {
      return{
        logo: logo,
        settings: settings,
        bell: bell,
        avatar: avatar,
        search: search,
        burger: burger
      }
    },

    components: {
      Button,
    }
  }
</script>

<template>
  <div class="d-flex px-5 navbar navbar-expand-lg bg-light">
    <a class="navbar-brand" href="#">
      <li class="nav-item d-flex logo">
        <img :src="logo"/>
        <a class="nav-link px-0" href="#">Untitled UI</a>
      </li>
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <img :src="burger">
    </button>
    <div class="navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto">
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Home</a> 
        </li>
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Dashboard</a>
        </li>
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Project</a>
        </li>
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Tasks</a>
        </li>
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Reporting</a>
        </li>
        <li class="nav-item px-2">
          <a class="nav-link" href="#">Users</a>
        </li>
      </ul>
      <ul class="navbar-nav">
        <Button />
        <li class="icon">
          <a href="#"><img class="px-2" :src="settings"></a>
        </li>
        <li class="icon">
          <a href="#"><img class="px-2" :src="bell"></a>
        </li>
        <li>
          <a href="#"><img class="px-2" :src="avatar"></a>
        </li>
      </ul>
    </div>
  </div>
    <div class="divider"></div>
    <div class="container-fluid px-5 py-2 d-flex navbar-collapse" id="navbarSupportedContent">
      <ul class="nav me-auto">
        <li class="nav-item">
          <a class="nav-link active" href="#">Overview</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Notification</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Analytics</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Saved reports</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Trade History</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">User reports</a>
        </li>
      </ul>
      <form>
        <div class="d-flex search justify-content-between">
          <img class="d-block search-icon" :src="search">
          <input class="input px-2 py-2 h-100" type="text" placeholder="Search" aria-label="Search">
        </div>
      </form>
    </div>

</template>



<style scoped>

nav {
  background: #FFFFFF !important;
}
.logo {
  padding-right: 10px;
  color: #101828 !important;
  width: 150px;
}

.nav-link {
  color: #344054;
  font-weight: 500;
  line-height: 24px;
}

.icon {
  padding: 5px 10px;
}

.search {
  background: #FFFFFF;
  border: 2px solid #D0D5DD;
  box-shadow: 0px 1px 2px rgba(16, 24, 40, 0.05);
  border-radius: 8px;
  width: 350px;
  padding-left: 10px;
}

.search-icon {
  height: 20px;
  width: 20px;
  top: 8px;
  border: none;
}

.input {
  background: #FFFFFF;
  border: none;
  width: 100%;
  margin-left: 5px;
}

.active {
  background: #F9FAFB;
  border-radius: 6px;
}
</style>