<template>
  <!--<HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>-->
  <PageHeader />
  <main>
    <PageSearch />
    <PageMenu />
  </main>
  <PageFooter />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import PageHeader from './components/PageHeader.vue'
import PageSearch from './components/PageSearch.vue'
import PageMenu from './components/PageMenu.vue'
import PageFooter from './components/PageFooter.vue'


@Options({
  components: {
    PageHeader,
    PageSearch,
    PageMenu,
    PageFooter,
  },
})
export default class App extends Vue {}
</script>

<style>
*, #app{
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  padding: 0;
}
html, body {
    background-color: #fff;
}
header {
    text-align: center;
    display: flex;
    height: 8vh;
    color: #fff;
    background-color: #000;
}
.lewy{
    flex: 1;
    padding: 5px;
    float: left;
    display: flex;
    align-items: center;
    padding-left: 5%;
}
.logo {
    height: 3vh;
    margin-right: 5px;
    float: left;
}
.prawy{
    flex: 1;
    padding: 7px;
    text-align: right;
    padding-right: 5%;
    
}
.request{
    background-color: #000;
    color: #fff;
    border-radius: 5px;
    border-color: #fff;
    padding: 10px;
    margin-right: 10px;
    padding-left: 10px;
    padding-right: 10px;
}
.singIn{
    background-color: #4C5FD5;
    color: #fff;
    border-radius: 5px;
    border: none;
    padding: 10px;
    padding-left: 10px;
    padding-right: 10px;
}
.wyszukiwarka {
    height: 22vh;
    background-color: #dadbf1;
    text-align: center;
}
.title {
    font-size: 50px;
    padding: 15px;
}
input[type="search"]{
    width: 50%;
    box-shadow: 0px 0px 4px #000;
    border: none;
    padding: 10px;
}
.menu {
    padding-top: 10px;
    height: 60vh;
    display: grid;
    grid-template-columns: repeat(2,1fr);
    grid-template-rows: repeat(2,100px);
}
.zawartosc {
    display: grid;
    grid-template-columns: 1fr 1fr;
}
div{
    font-size: 11px;
    padding: 10px;
}
.pictures {
    height: 10vh;
}
div img{
    float: right;
}
a{
    text-decoration: none;
}

footer {
    height: 140px;
    color: #fff;
    background-color: #000;
    display: flex;
    position: absolute;
    width: 100%;
    bottom: 0;
}
.margin {
    flex: 1;
}
.content {
    display: flex;
}
.footer1, .footer2, .footer3, .footer4, .footer5{
    flex: 1;
    padding: 10px;
    font-size: 12px;
}
.footer1 {
    padding-left: 10%;
}
.footer5 {
    padding-right: 10%;
}
h3, h4 {
    margin: 0px;
}
h3 {
    padding-bottom: 5px;
}
.footer5 {
    padding-top: 50px;
}

</style>
