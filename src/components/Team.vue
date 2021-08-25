<template>
  <section id="zespol">
    <h4>Poznaj naszą załogę</h4>
    <div class="team">
      <div v-for="teamMember in team" :key="teamMember.id" class="team--member">
        <img :src="teamMember.image" />
        <p>{{ teamMember.name }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Team",
  data() {
    return {
      team: [
        {
          id: 1,
          name: "Michał",
          image: require("../assets/barbers/michal.jpg"),
        },
        {
          id: 2,
          name: "Adam",
          image: require("../assets/barbers/adam.jpg"),
        },
        {
          id: 3,
          name: "John",
          image: require("../assets/barbers/john.jpg"),
        },
        {
          id: 4,
          name: "Anna",
          image: require("../assets/barbers/anna.jpg"),
        },
        {
          id: 5,
          name: "Kamil",
          image: require("../assets/barbers/kamil.jpg"),
        },
      ],
    };
  },
};
</script>

<style scoped>
#zespol {
  background: #000;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 10rem 0rem;
}
.team {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
  width: 80%;
  /* margin-bottom: 50px; */
}

.team--member {
  width: 400px;
  height: 400px;
  text-align: center;
  padding: 40px 20px 20px 20px;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

p {
  color: #e7ecef;
  text-transform: uppercase;
  letter-spacing: 2px;
  margin: 1rem 0rem;
}

h4 {
  font-style: italic;
  color: #e7ecef;
}

h4::before {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #b59472;
  margin: 0px 14px 4px;
}

h4::after {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #b59472;
  margin: 0px 14px 4px;
}
</style>
