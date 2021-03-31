<template>
     <section class="securities">
      <div class='container'>
        <div class="row text-center">
          <div class="col-sm">
            <h2 id='securities'>What Are Digital Securities?</h2>
            <p>Digital securities represent traditional assets like equity or bonds.<br>
              They carry all of the same legal rights of their paper issued counter-parts.
            </p>
          </div>
        </div>
        <div class="row align-items-center items">
          <div class="col-sm text-center item1">
            <img src="../assets/images/Group1.png" alt="">
            <h3>Invest Any Amount </h3>
            <p>Start with as little as $1,<br>
               buy parts of a whole share </p>
          </div>
          <div class="col-sm text-center item2">
            <img src="../assets/images/Group2.png" alt="">
            <h3>Access Private Equity</h3>
            <p>Get access to investments<br>
              typically reserved for institutions</p>
          </div>
          <div class="col-sm text-center item3">
            <img src="../assets/images/Group3.png" alt="">
            <h3>Trade 24/7</h3>
            <p>Digital assets don’t sleep,<br>
               so why should you stop trading?</p>
          </div>
        </div>
        <div class="row align-items-center">
          <div class="col-sm text-center">
            <form class="align-self-center">
              <input class="form-control me-2 email" type="email" placeholder="E-mail" aria-label="Search">
              <button class="btn btn-sm email" type="submit">Get Early Access</button>
            </form>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'Securities'
}
</script>

<style scoped lang="scss">
  section.securities{
    padding-top: 35px;
}
h2{
    font-weight: 600;
    font-size: 45px;
    line-height: 61px;
    color: #000000;
    text-transform: capitalize;
}
h3{
    font-weight: 600;
    font-size: 30px;
    line-height: 41px;
}
.securities p,
.products p{
    font-size: 24px;
    line-height: 34px;
    color: #000000;
}
.securities p{
    margin-top: 17px;
}
.securities .items{
    margin-top: 40px;
}
.securities h3{
    margin-top: 35px;
}
.securities form{
    margin: 0 auto;
    margin-top: 10px;
    margin-bottom: 33px;
}
input.email{
    display: inline-block;
    max-width: 445px;
    padding: 12px;
    border-radius: 10px;
}
button.email {
    display: inline-block;
    margin-left: 20px;
    padding: 10px 46px;
    color: #fff;
    font-size:20px;
    line-height:27.24px;
    font-weight: 600;
    background: #2ECC71;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.15);
    border-color: #2ECC71;
    border-radius: 10px;
}
button.email:hover {
    background: #FFFFFF;
    color:#2ECC71;
}
@media screen and (max-width: 375px){
    .securities .items {
        margin-top: 0px;
    }
    section.securities{
        height: auto;
        padding-top: 16px;
    }
    h2{
        font-size: 35px;
        line-height:32px;
    }
    h3{
        font-size: 22px;
        line-height: 30px;
    }
    .securities p,
    .products p{
        font-size: 18px;
        line-height: 25px;
    }
    .item1 img{
        width: 55%;
    }
    .item1 img ~ h3{
        margin-top: 27px;
    }
    .item2 img{
        width: 67%;
        margin-top: 10px;
    }
    .item2 img ~ h3 {
        margin-top: 37px;
    }
    .item3 img{
        width: 62%;
        margin-top: 3px;
    }
    .item3 img ~ h3 {
        margin-top: 32px;
    }
    .securities form {
        margin-bottom: 0;
    }
    button.email {
        margin-top: 13px;
        margin-bottom: 40px;
        width: 100%;
        margin-left: 0px;
    }
}
@media screen and (min-width: 376px) and (max-width: 991px){
    button.email{
        margin-top: 20px;
        margin-left: 0px;
    }
}
</style>
