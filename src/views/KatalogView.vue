<template>
  <div class="qwe">
    <div class="card" v-for="computer in computers" :key="computer.id">
      <div class="card-item">
        <img :src="computer.image" alt="RTX4090" style="width:100%" id="k1">
        <a> {{ computer.name }} </a>
        <p class="price">140.000р</p>
        <p>Игровой Компьютер</p>
        <div class="opisanie"> GPU: {{ computer.gpu }}</div>
        <div class="cpu">CPU: {{ computer.cpu }}</div>
        <div class="knop">Подробнее</div>

      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'KatalogView',
  data: () => {
    return {
      computers: [
        {
          id: 1,
          name: "VALIEVA CYBER",
          cpu: "Intel® Core™ i7-12700F",
          gpu: "GeForce RTX 3080TI 12GB",
          ram: "16GB DDR4",
          mb: "MSI MPG B660",
          bp: "1000W",
          ssd: "1TB Samsung 970",
          image: 'https://c.dns-shop.ru/thumb/st4/fit/760/600/da6db1b326fb9756feaf17e782f2acc8/q93_4f1b7d3b3137413c08e108d4284c3c715cfdfdde6eda44f619287b6cc69eb184.jpg'
        },
        {
          id: 2,
          name: "Cyber",
          cpu: "Intel® Core™ i7-12700F",
          gpu: "GeForce RTX 3080TI 12GB",
          ram: "16GB DDR4",
          mb: "MSI MPG B660",
          bp: "1000W",
          ssd: "1TB Samsung 970",
          image: 'https://c.dns-shop.ru/thumb/st4/fit/760/600/da6db1b326fb9756feaf17e782f2acc8/q93_4f1b7d3b3137413c08e108d4284c3c715cfdfdde6eda44f619287b6cc69eb184.jpg'
        },
        {
          id: 3,
          name: "Cyber",
          cpu: "Intel® Core™ i7-12700F",
          gpu: "GeForce RTX 1090TI 12GB",
          ram: "16GB DDR4",
          mb: "MSI MPG B660",
          bp: "500W",
          ssd: "1TB Samsung 970",
          image: 'https://c.dns-shop.ru/thumb/st4/fit/760/600/da6db1b326fb9756feaf17e782f2acc8/q93_4f1b7d3b3137413c08e108d4284c3c715cfdfdde6eda44f619287b6cc69eb184.jpg'
        }
        
        
      ]
    }
  }
}
</script>
<style>
.qwe {
  border: red solid 1px;
  display: grid;
  grid-template-columns: 0.5fr 0.5fr 0.5fr;
  justify-items: center;
  gap: 0px;
}

.card {
  box-shadow: -6px 10px 20px 0 pink;
  max-width: 300px;
  position: relative;
  margin-top: 10%;
  text-align: center;
  font-family: arial;

}

.price {
  color: grey;
  font-size: 22px;
}

.knop {
  border: none;
  outline: 0;
  padding: 12px;
  color: orange;
  background-color: rgb(15, 15, 15);
  text-align: center;
  width: 92%;
  font-size: 20px;
  font-weight: bolder;
}



p {
  color: black;
  font-family: Verdana;
}

.cont {
  position: absolute;
  margin-top: 5%;
  margin-left: 20%;
  display: flex;
  flex-direction: center;
  margin-right: 200px;
  width: 60%;
  justify-content: space-around;
  flex-wrap: wrap;


}

.tow {
  color: black;
}

.card:hover {
  box-shadow: -2px 4px 100px purple;

}

.opisanie {
  padding-left: 5px;
  text-align: left;
  line-height: 32px;
}

h3 {
  color: black;

}
</style>