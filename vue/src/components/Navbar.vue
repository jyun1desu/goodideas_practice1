<template>
    <nav>
        <h1 class="logo">
        <img :src="logo.src" alt="logo商標" />
        <span>ZERO TYPE</span>
        </h1>
        <div class="menu">
        <a  v-for="link in linkList" 
            href="#" 
            :key="link.title">
            {{ link.title }}
        </a>
        </div>
    </nav>
</template>

<script>
    export default {
    data() {
        return {
        logo:{
            brandName: "ZERO TYPE",
            src: require('../assets/logo.png')
        },
        linkList: [
            { title: "Home", url: "#" },
            { title: "Features", url: "#" },
            { title: "News", url: "#" },
            { title: "About", url: "#" },
            { title: "Contact", url: "#" },
        ],
        };
    },
    };
</script>

    <style>
nav {
  font-size: 0;
}

.logo {
  display: inline-block;
  vertical-align: middle;
  text-align: center;
}

.logo img {
  display: block;
  width: 55px;
  margin: 0 auto;
}

.logo_image img {
  width: 100%;
}

.logo span {
  font-size: 16px;
  color: #333;
  font-weight: 700;
}

.menu {
  display: inline-block;
  vertical-align: middle;
  margin: 0 72px;
}

.menu a {
  display: inline-block;
  font-size: 17px;
  text-decoration: none;
  color: #888;
  padding: 10px 0;
}

.menu a + a {
  margin-left: 103px;
}

a:hover {
  color: orange;
}
</style>