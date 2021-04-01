<template>
    <section class = 'products'>
      <div class="container">
        <div class="wrapper">
          <h2 class = 'products-title'>Products</h2>
        </div>
        <div class="wrapper">
          <div class="content">
            <button class="launchpad" >Launchpad</button>
            <p>Help launch startups<br>
               & fund private bussinesses</p>
            <button class="marketplace">Marketplace</button>
            <p>Browse through stocks on sale<br>
              from private investors</p>
          </div>
          <div class="content">
            <img src="../assets/images/EQTZ 1.jpg" alt="">
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'Products'
}
</script>

<style scoped lang="scss">
  .products-title{
    margin-top: 60px;
  }
  .products .wrapper{
    align-items: center;
  }
  .products .content{
    text-align: center;
    flex: 1 0 0;
  }
  .products p{
      margin-top: 10px;
      letter-spacing: 0.5px;
  }
  button.launchpad,
  button.marketplace{
      margin-top: 20px;
      box-sizing: border-box;
      width: 350px;
      height: 78px;
      border-radius: 10px;
      font-size: 32px;
      line-height: 44px
  }
  button.launchpad:hover{
      color:#2ECC71;
  }
  button.marketplace:hover{
      color:#252525;
  }
  button.launchpad{
      margin-top: 20px;
      color:#252525;
      border: 5px solid #252525;
  }
  button.marketplace{
      margin-top:50px;
      color:#2ECC71;
      border: 5px solid #2ECC71;
  }
  @media screen and (max-width: 375px){
    .products-title{
      margin-top: 50px;
    }
    button.marketplace,
    button.launchpad{
      margin-top: 15px;
      font-size: 25px;
      line-height: 34px;
      height: 63px;
      width: 100%;
      border-width: 3px;
    }
  }
  @media screen and  (min-width: 280px) and (max-width: 374px){
    .products img {
          width: 260px;
      }
  }
</style>
