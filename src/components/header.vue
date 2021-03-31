<template>
 <header>
        <nav class="navbar navbar-expand-lg navbar-light">
            <div class="container">
              <a class="navbar-brand" href="#">
                <img src="../assets/images/Equiteez.svg" alt="Equiteez" width="179px" height="51px">
              </a>
              <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                <div class="navbar-nav">
                  <a class="nav-link" href="#securities">What Are Digital Securities?</a>
                  <a class="nav-link" href="#products">Products</a>
                  <a class="nav-link" href="#">Digitize Your Business</a>
                  <a class="nav-link" href="#">Blog</a>
                  <a class="nav-link" href="#">Contact Us</a>
                </div>

                <ul class="navbar-nav flex-row flex-wrap ms-md-auto">
                  <li class="nav-item col-6 col-md-auto">
                    <a class="nav-link p-2" href="#" target="_blank" rel="noopener">
                      <img src="../assets/images/Twitter (Traced).svg" alt="Equiteez" width="30px" height="30px">
                      <small class="d-md-none ms-2"></small>
                    </a>
                  </li>
                  <li class="nav-item col-6 col-md-auto">
                      <a class="nav-link p-2" href="#" target="_blank" rel="noopener">
                          <img src="../assets/images/Facebook (Traced).svg" alt="Equiteez" width="30px" height="30px">
                          <small class="d-md-none ms-2"></small>
                      </a>
                    </li>
                    <li class="nav-item col-6 col-md-auto">
                      <a class="nav-link p-2" href="#" target="_blank" rel="noopener">
                          <img src="../assets/images/Linkedin (Traced).svg" alt="Equiteez" width="30px" height="30px">
                          <small class="d-md-none ms-2"></small>
                      </a>
                    </li>
                    <li class="nav-item col-6 col-md-auto">
                      <a class="nav-link p-2" href="#" target="_blank" rel="noopener">
                          <img src="../assets/images/Medium.svg" alt="Equiteez" width="30px" height="30px">
                          <small class="d-md-none ms-2"></small>
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
header a.nav-link{
    font-weight: 600;
    font-size: 18px;
    line-height: 25px;
    color:#000000;
}
header a:hover{
    text-decoration: underline;
}
@media screen and (max-width: 375px){
    .navbar-brand{
        margin: 0 auto;
    }
}
</style>
