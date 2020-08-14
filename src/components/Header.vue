<template>
<div class="header">
   <div class="topnav" id="myTopnav">
    <a href="#about" class="active">Eldoret js</a>
    <a href="#services">Our Services</a>
    <a href="#location">Our Location</a>
    <a href="#events">Events</a>
    <a href="#members">Team</a>
    <a href="#about">Register</a>
    <a href="javascript:void(0);" class="icon" @click="showMenu()">
    <i class="fa fa-bars"></i>
    </a>
 </div> 
</div>

</template>

<script>
export default {
  name: "Header",
  components: {},
  methods: {
    showMenu() {
      let topNav = document.getElementById("myTopnav");
      if (topNav.className === "topnav") {
         return topNav.className += " responsive";
      } else {
        return topNav.className = "topnav";
      }
    }
  }
}
</script>

<style scoped>
.topnav {
  overflow: hidden;
  background-color:#ff9e15;
  padding: 10px;
}

.topnav a {
  float: left;
  display: block;
  color: #fff;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  font-family:Poppins;
  font-weight:500;
  display:swap;
  margin-left: 10px;
}

.topnav a:hover {
  /* background-color: #ddd; */
  color: #99381f;
  text-decoration: underline;
  transition: ease-in-out 500ms;
  
}

.topnav .icon {
  display: none;
}
.search{
    width: 15%;
    box-sizing: border-box;
    border: 2px solid #ccc;
    border: none;
    float: right;
    margin-right: 50px;
    /* padding: 20px; */
    font-size: 16px;
    background-color: white;
    background-position: 10px 10px;
    background-repeat: no-repeat;
    padding: 13px 20px 12px 20px;
    -webkit-transition: width 0.4s ease-in-out;
    transition: width 0.4s ease-in-out;
}

@media screen and (max-width: 600px) {
  .topnav a:not(:first-child) {display: none;}
  .topnav a.icon {
    float: right;
    display: block;
    color: #fff;
    font-size: 28px;
  }
}

@media screen and (max-width: 600px) {
  .topnav.responsive {position: relative;}
  .topnav.responsive .icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .topnav.responsive a {
    float: none;
    display: block;
    text-align: left;
    height: 1vh;
    margin-top: -5px;
  }
  .active{
    text-transform: uppercase;
  }
}
</style>