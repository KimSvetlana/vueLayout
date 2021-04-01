<template>
    <header id ='header' class='header'>
    <div class='container'>
        <div class='header-body'>
            <div id='#toggle' class='header-burger'  :class="{activeBur: isActive}" @click="show">
                <span></span>
            </div>
            <div class='header-logo'>
                <a><img src="../assets/images/Equiteez.svg" alt="Equiteez" width="179px" height="51px"></a>
            </div>
      <nav class='header-menu' id='bar' :class="{activeBur: isActive}">
          <ul class='header-list'>
              <li><a class="header-link" href="#securities">What Are Digital Securities?</a></li>
                <li><a class="header-link" href="#products">Products</a></li>
                <li><a class="header-link" href="#">Digitize Your Business</a></li>
                <li><a class="header-link" href="#">Blog</a></li>
                <li><a class="header-link" href="#">Contact Us</a></li>
            </ul>
          <ul class="header-list social">
                  <li>
                    <a href="#">
                      <img src="../assets/images/Twitter (Traced).svg"  width="30px" height="30px">
                    </a>
                  </li>
                  <li>
                      <a href="#">
                          <img src="../assets/images/Facebook (Traced).svg"  width="30px" height="30px">
                      </a>
                    </li>
                    <li>
                      <a href="#">
                          <img src="../assets/images/Linkedin (Traced).svg" alt="Equiteez" width="30px" height="30px">
                      </a>
                    </li>
                    <li>
                      <a href="#">
                          <img src="../assets/images/Medium.svg" width="30px" height="30px">
                      </a>
                    </li>
                </ul>
      </nav>
    </div>
  </div>
</header>
</template>

<style scoped lang="scss">

.container{
    padding: 0 20px;
}

.header::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 105px;
    background-color: #FFFFFF;
    box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.25);
    z-index: 6;
}
.header-body{
    position: relative;
    box-sizing: border-box;
    display: flex;
    justify-content: space-between;
    text-align: center;
    align-items: center;
    height: 105px;
    align-items: center;
    width: 100%;
    background-color: white;
};

.header-logo{
    position: relative;
    z-index: 7;
}
.header-burger{
    display: none;
}
.header-menu {
    display: flex;
    flex-wrap: inherit;
    align-items: center;
    justify-content: space-between;
}
.header-list {
    display: inherit;
    position: relative;
    z-index: 6;
    list-style: none;
}
.list_item{
    float: left;
    overflow: hidden;
}
.social{
    margin-top: 0;
    margin-left: auto ;

    & a{
        padding: 0 0.5rem;
    }
  }

.header-link{
    color: #000000;
    text-decoration: none;
    padding: 0 0.5rem;
    position: relative;
    &:hover{
        text-decoration: underline;
    }
}
@media(max-width: 992px){
    .header-logo{
        margin: 0 auto;
        & img{
            width: 146px;
            height: 39px;
        }
    }
    .header-burger{
        position: relative;
        display: block;
        width: 23px;
        height: 15px;
        z-index: 7;
    }
    .header-burger::before,
    .header-burger::after{
        content: '';
        position: absolute;
        background-color: #2ECC71;
        width: 100%;
        height: 3px;
        left:0;
        transition: all 0.3s ease 0s;
    }
    .header-burger::before{
        top: 0;
    }
    .header-burger::after{
        bottom:0;
    }
    .header-burger.activeBur::before{
        transform: rotate(45deg);
        top: 6px;
    }
    .header-burger.activeBur::after{
        transform: rotate(-45deg);
        bottom: 6px;
    }
    .header-burger span{
        position: absolute;
        background-color: #2ECC71;
        width: 100%;
        height: 3px;
        left: 0;
        top: 6px;
        transition: all 0.3s ease 0s;
    }
    .header-burger.activeBur span{
        transform: scale(0);
    }
    .header-menu{
        position: fixed;
        z-index: 5;
        top:-150%;
        left:0;
        width: 100%;
        height: 100%;
        background-color: rgb(165, 207, 247);
        padding: 105px 0 0 0;
        transition: all 0.3s ease 0s;
        overflow: auto;
    }
    .header-menu.activeBur{
        display:initial;
        top:0;
    }
    .activeBur .header-list li{
        margin: 30px;
    }

}
</style>
<script>
// import Vue from 'vue'
export default {

  el: 'header',
  data: function () {
    return {
      isActive: false
    }
  },
  methods: {
    show: function () {
      this.isActive = !this.isActive
    }
  }

}
</script>
