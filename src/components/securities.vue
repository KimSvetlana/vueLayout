<template>
     <section class="securities">
      <div class='container'>
        <div class="wrapper">
          <div class="content">
            <h2 id='securities'>What Are Digital Securities?</h2>
            <p>Digital securities represent traditional assets like equity or bonds.<br>
              They carry all of the same legal rights of their paper issued counter-parts.
            </p>
          </div>
        </div>
        <div class="wrapper items">
          <div class="content item1">
            <img src="../assets/images/Group1.png" alt="">
            <h3>Invest Any Amount </h3>
            <p>Start with as little as $1,<br>
               buy parts of a whole share </p>
          </div>
          <div class="content item2">
            <img src="../assets/images/Group2.png" alt="">
            <h3>Access Private Equity</h3>
            <p>Get access to investments<br>
              typically reserved for institutions</p>
          </div>
          <div class="content item3">
            <img src="../assets/images/Group3.png" alt="">
            <h3>Trade 24/7</h3>
            <p>Digital assets don’t sleep,<br>
               so why should you stop trading?</p>
          </div>
        </div>
        <div class="wrapper">
          <div class="content form">
            <form>
              <input class="email" type="email" placeholder="E-mail" aria-label="Search">
              <button class="email" type="submit">Get Early Access</button>
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
    .securities .wrapper{
        text-align: center;
    }
    .securities .content{
        flex: 1 0 0%;
    }
    .item1, .item2, .item3{
        text-align: center;
    }
    .securities p{
        margin-top: 15px;
    }
    .securities .items{
        margin-top: 40px;
        align-items: center;
    }
    .securities h3{
        margin-top: 35px;
    }
    .content .form{
        align-items: center ;
        flex: 1 0 0%;
    }
    .securities form{
        margin: 0 auto;
        margin-top: 10px;
        margin-bottom: 33px;
    }
    input.email{
        display: inline-block;
        max-width: 445px;
        width: 100%;
        padding: 12px;
        border-radius: 10px;
        font-size: 1rem;
        font-weight: 400;
        line-height: 1.5;
        color: #212529;
        background-color: #fff;
        background-clip: padding-box;
        border: 1px solid #ced4da;
        border-radius: 0.5rem;
        transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;

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
        border: 1px solid transparent;
        border-color: #2ECC71;
        border-radius: 10px;
    }
    button.email:hover {
        background: #FFFFFF;
        color:#2ECC71;
    }
    @media screen and (max-width: 375px){
        .items .content{
            flex:none;
        }
        .item1, .item2, .item3{
            width: 100%;
        }
        .securities .items {
            margin-top: 25px;
        }
        section.securities{
            height: auto;
            padding-top: 16px;
        }
        .item1 img{
            width: 55%;
        }
        .item1 img ~ h3{
            margin-top: 20px;
        }
        .item2 img{
            width: 67%;
            margin-top: 28px;
        }
        .item2 img ~ h3 {
            margin-top: 33px;
        }
        .item3 img{
            width: 62%;
            margin-top: 17px;
        }
        .item3 img ~ h3 {
            margin-top: 29px;
        }
        .securities form {
            margin-top: 27px;
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
