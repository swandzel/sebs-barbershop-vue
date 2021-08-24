<template>
  <nav>
    <div class="navbar">
      <div class="logo">
        <!-- <img src="../assets/barber.svg" color="#fff" width="30" /> -->
        Seb's Barbershop
      </div>
      <ul class="navbar--links">
        <li v-for="link in links" :key="link.id">
          <a :href="link.link">{{ link.name }}</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      links: [
        { id: 1, name: "Start", link: "#start" },
        { id: 2, name: "O nas", link: "#o-nas" },
        { id: 3, name: "Oferta", link: "#oferta" },
        { id: 4, name: "Zespół", link: "#" },
        { id: 5, name: "Szkolenia", link: "#" },
        { id: 6, name: "Prasa", link: "#" },
        { id: 7, name: "Kontakt", link: "#" },
      ],
    };
  },
};
</script>

<style scoped>
nav {
  display: flex;
  flex-direction: row;
  justify-content: center;
  position: absolute;
  width: 100%;
  font-family: "Lora", serif;
  font-size: 1.25rem;
  color: #e7ecef;
}

.navbar {
  display: flex;
  flex-direction: row;
  width: 1500px;
  height: 100px;
  justify-content: space-around;
  align-items: center;
}

.logo {
  font-family: "Gloria Hallelujah", cursive;
  font-size: 2rem;
}

.navbar--links {
  display: flex;
  flex-direction: row;
}

.navbar--links li {
  list-style: none;
  padding: 0px 10px;
}

.navbar--links li a {
  color: #e7ecef;
  text-decoration: none;
}

.navbar--links li a:hover {
  text-decoration: underline;
}
</style>
