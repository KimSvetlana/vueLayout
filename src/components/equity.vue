<template>
    <section class='equity'>
        <div class="container">
            <div class="wrapper">
                <div class='content'>
                    <h1>Private Equity Made Easy</h1>
                    <img class='phone' src="../assets/images/001.png">
                    <img class='phone-shadow' src="../assets/images/Ellipse 11.png" alt="">
                    <p>Equiteez is on a mission to make private equity easily accesible to all in vestors</p>
                    <button type="button" class="singnup">Singnup For Free</button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Equity'
}
</script>

<style scoped lang="scss">
    section.equity{
        overflow: hidden;
        height: 768px;
        background-color: #2ECC71;
    }
    .equity h1 {
        margin-top: 17px;
        font-size: 52px;
        line-height: 71px;
        font-weight: bold;
        color: #FFFFFF;
        letter-spacing: 1px;
    }
    .equity p{
        margin-top: 30px;
        width: 635px;
        font-size: 32px;
        line-height: 44px;
        color: #FFFFFF;
        letter-spacing: 0.5px;
    }
    .equity .singnup {
        margin-top: 35px;
        padding: 14px 44px;
        color: #fff;
        font-size:20px;
        line-height:27.24px;
        font-weight: 600;
        background: #252525;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.15);
        border: 1px solid #252525;
        border-radius: 10px;
    }
    .equity .singnup:hover{
        background: #fff;
        color:#252525;
    }
    .equity .content {
        position: relative;
        margin-top: 200px;
    }
    .equity .phone{
        position: absolute;
        top: -235px;
        left: 430px;
        z-index: 3;
    }
    .equity .phone-shadow{
        position:absolute;
        top: 50px;
        left: 660px;
        z-index: 1;
    }

    @media screen and (max-width: 375px){
        section.equity{
            height:auto;
        }
        .equity h1 {
            margin-top: 8px;
            font-size: 35px;
            line-height: 40px;
            text-align: center;
        }
        .equity p{
            margin-top: -158px;
            padding: 0 30px;
            width:auto;
            font-size: 22px;
            line-height: 25px;
            text-align: center;
        }
        .equity .content{
            margin-top: 0px;
            text-align: center;
        }

        .equity .phone{
            position: relative;
            width: 170%;
            top: -80px;
            left: -60px;
        }
        .equity .phone-shadow{
            top: 150px;
            left: 10px;
        }
        .equity .singnup {
            margin-top: 14px;
            margin-bottom: 37px;
        }
    }
    @media screen and (min-width: 376px) and (max-width: 991px){
        section.equity{
            height: auto;
        }
        .equity .phone{
            position:static;
        }
        .equity .phone-shadow {
            top: 380px;
            left: 140px;
        }
        .equity .content {
            width: 100%;
            margin-top: 0;
            text-align: center;
        }
        .equity p {
            margin-top: -60px;
            width: auto;
        }
        .equity .singnup{
            margin-top: 0;
            margin-bottom: 20px;
        }
    }
    @media screen and  (min-width: 280px) and (max-width: 374px){
        .equity p {
            margin-top: -140px;
        }
        .equity .phone{
            top: -65px;
            left: -90px;
        }
        .equity .phone-shadow{
            top: 200px;
            left: 40px;
            width: 100%;
        }
    }
</style>
