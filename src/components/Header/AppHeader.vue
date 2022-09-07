<template>
  <div>
    <CounterSection/>
    <div class="container-navbar">
      <a href="">
        <img src="@/images/dark-logo.png" alt="logo">
      </a>

      <ul>
        <li v-for="(link, index) in listNav" :key="index">
          <div class="dropdown">
            <div>
              {{link.title}}
              <i class="fas fa-angle-down"></i>
            </div>
            <div class="dropdown-content">
              <a href="">{{link.link1}}</a>
              <a href="">{{link.link2}}</a>
              <a href="">{{link.link3}}</a>
              <a href="">{{link.link4}}</a>
            </div>
          </div>
        </li>
      </ul>

      <div>
        <a href=""><i class="fa-brands fa-twitter"></i></a>
        <a href=""><i class="fa-brands fa-facebook-f"></i></a>
        <a href=""><i class="fa-brands fa-instagram"></i></a>
        <a href=""><i class="fa-brands fa-linkedin"></i></a>
      </div>
    </div>
    <HeroSection/>
  </div>
</template>

<script>
import CounterSection from './CounterSection.vue';
import HeroSection from './HeroSection.vue';

export default {
    name: "AppHeader",

    components: { 
      CounterSection, 
      HeroSection 
    },
    data(){
      return{
        listNav:[
          {
            title: 'Home',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          },
          {
            title: 'Pages',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          },
          {
            title: 'Courses',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          },
          {
            title: 'Features',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          },
          {
            title: 'Blog',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          },
          {
            title: 'Shop',
            link1: 'test',
            link2: 'test',
            link3: 'test',
            link4: 'test'
          }
        ]
      }
    }
}
</script>

<style lang="scss">
.container-navbar{
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 70px;

    .dropdown {

      .fa-angle-down{
        font-size: 10px;
      }

      .dropdown-content {
        display: none;
        position: absolute;
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        z-index: 1;
      }
      .dropdown-content a {
        color: black;
        text-decoration: none;
        display: block;
        padding: 5px 20px;
        text-align: left;
      }
    }
    .dropdown:hover .dropdown-content{
      display: block;
    }

    img{
      height: 30px;
    }
    
    ul{
      display: flex;
        li{
          list-style: none;
          padding: 0 15px;
          font-size: 14px;
          font-weight: 400;
        }
    }
    div a{
      padding:0 10px;
      color: rgb(105, 105, 105);
    }
}
</style>