<template>
 <header>
        <nav class="navbar">
            <div class="container">
              <a class="navbar-brand" href="#">
                <img src="../assets/images/Equiteez.svg" alt="Equiteez" width="179px" height="51px">
              </a>
              <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button> -->
              <div class="navbar-collapse">
                <div class="navbar-nav">
                  <a class="nav-link" href="#securities">What Are Digital Securities?</a>
                  <a class="nav-link" href="#products">Products</a>
                  <a class="nav-link" href="#">Digitize Your Business</a>
                  <a class="nav-link" href="#">Blog</a>
                  <a class="nav-link" href="#">Contact Us</a>
                </div>

                <ul class="navbar-nav social">
                  <li class="nav-item">
                    <a class="nav-link " href="#">
                      <img src="../assets/images/Twitter (Traced).svg"  width="30px" height="30px">
                    </a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#">
                          <img src="../assets/images/Facebook (Traced).svg"  width="30px" height="30px">
                      </a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link" href="#">
                          <img src="../assets/images/Linkedin (Traced).svg" alt="Equiteez" width="30px" height="30px">
                      </a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link" href="#">
                          <img src="../assets/images/Medium.svg" width="30px" height="30px">
                      </a>
                    </li>
                </ul>
              </div>
            </div>
          </nav>
    </header>

</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header nav {
    height: 105px;
    background: #FFFFFF;
    box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.25);
  }
  .navbar{
    position: relative;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  .navbar > .container{
    display: flex;
    flex-wrap: inherit;
    align-items: center;
    justify-content: space-between;
  }
  .navbar-nav {
    display: flex;
    flex-direction: column;
    padding-left: 0;
    margin-bottom: 0;
    list-style: none;
  }
  @media (min-width: 992px){
    .navbar{
      flex-wrap: nowrap;
      justify-content: flex-start;
    }
    .navbar-nav {
      flex-direction: row;
    }
  }
  .navbar-brand {
    padding-top: 0.3125rem;
    padding-bottom: 0.3125rem;
    margin-right: 1rem;
    font-size: 1.25rem;
    text-decoration: none;
    white-space: nowrap;
  }
  .navbar-collapse {
    display: flex;
    flex-basis: 100%;
    flex-grow: 1;
    align-items: center;
  }
  .nav-link{
    padding-right: 0.5rem;
    padding-left: 0.5rem;
  }
  header a.nav-link{
    font-weight: 600;
    font-size: 18px;
    line-height: 25px;
    color:#000000;
    text-decoration: none;
  }
  header a:hover{
    text-decoration: underline;
  }
  .social{
    margin-top: 0;
    margin-left: auto ;
  }
  @media screen and (max-width: 375px){
    .navbar-brand{
      margin: 0 auto;
    }
  }
</style>
