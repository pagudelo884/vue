<script>
export default {
    data() {
        return {
            title : 'This is My Title for Monday',
            person : {
            id: 1,
            name: 'Bill',
            img: 'https://www.alohacriticon.com/wp-content/uploads/2004/01/bill-murray-cazafantasmas-foto.jpg'
            },
            msg: "Bill uno de los integrantes de los cazafantasmas",
        }
    },
};
</script>

<template>
  <div>
    <h3>{{title}}</h3>
    <div :id="person.id">
        <h4>{{ person.name }}</h4>
        <img :src="person.img" :alt="person.name">
    </div>
    <h5>{{ msg }}</h5>
    <h5 v-html="msg"></h5>
  </div>
</template>

<style lang="css" scoped>
h3{
    color:magenta;
}
</style>
