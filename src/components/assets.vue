<template>
    <section class='assets'>
        <div class="container">
            <div class="wrapper">
             <div class="content">
                <p>
                    Digital Assets are the future of private equity <br> - Deloitte
                </p>
             </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Assets'
}
</script>

<style scoped lang="scss">
    section.assets{
        background-color: #252525;
    }
    .assets .wrapper{
        text-align: center;
    }
    .assets .content{
        width: 100%;
    }
    section.assets p {
        padding: 47px;
        margin-bottom: 0;
        font-weight: 600;
        font-size: 32px;
        line-height: 44px;
        color: #2FCC71;
    }
    @media screen and (max-width: 375px){
        section.assets p{
            padding: 26px 14px;
            font-size: 22px;
            line-height: 30px;
            font-weight: normal;
        }
    }
</style>
