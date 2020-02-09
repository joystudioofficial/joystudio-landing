<template>
  <div>
    <footer class="js-footer">
      <div class="container">
        <div class="row">
          <div class="column column-50 column-left">
            <div class="footer-copyright">
              <span class="copyright">
                &copy; Joy Studio {{ new Date().getFullYear() }}
              </span>
              <span class="contact">
                joystudiosofficial@gmail.com
              </span>
            </div>
          </div>
          <div class="column column-50 column-right">
            <ul class="js-social-media">
              <li>
                <a href="https://www.facebook.com/joystudioofficial/" target="_blank">
                  <img src="@/assets/images/social-media/facebook.svg" title="facebook" alt="" srcset="">
                </a>
              </li>
              <li>
                <a href="https://www.instagram.com/joystudio.official/" target="_blank">
                  <img src="@/assets/images/social-media/instagram.svg" title="instagram" alt="" srcset="">
                </a>
              </li>
              <li>
                <a href="https://github.com/joystudioofficial" target="_blank">
                  <img src="@/assets/images/social-media/github.svg" title="github" alt="" srcset="">
                </a>
              </li>
            </ul>
          </div>
        </div>

      </div>
    </footer>
  </div>
</template>

<style scoped>
  @media (min-width: 62rem) {
    .js-footer {
      width: 100%;
      border-top: 1px solid #e2e2e2;
    }

    .js-footer .container {
      padding: 5rem;
    }

    .js-footer .container .footer-copyright {
      float: left;
      text-align: left;
    }

    .js-footer .container .footer-copyright span {
      color: #888;
      display: block;
    }

    .js-footer .container .js-social-media {
      float: right;
      display: flex;
    }

    .js-footer .container .js-social-media li {
      list-style: none;
      margin: auto 1.5rem;
    }

    .js-footer .container .js-social-media li a img {
      width: 2rem;
      -webkit-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -moz-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -o-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -webkit-filter: grayscale(100%);
      -moz-filter: grayscale(100%);
      -o-filter: grayscale(100%);
      filter: grayscale(100%);
    }

    .js-footer .container .js-social-media li a img:hover {
      -webkit-transform: scale(1.1);
      -moz-transform: scale(1.1);
      -o-transform: scale(1.1);
      transform: scale(1.1);
    }
  }
  
  @media (max-width: 61.9375rem) {
    .js-footer {
      width: 100%;
      border-top: 1px solid #e2e2e2;
    }

    .js-footer .container {
      padding: 5rem;
    }

    .js-footer .container .row {
      align-content: center;
      justify-content: center;
    }

    .js-footer .container .row .column.column-50 {
      max-width: 100%;
    }

    .js-footer .container .row .column {
      margin: 2rem auto;
    }

    .js-footer .container .footer-copyright {
      text-align: center;
    }

    .js-footer .container .footer-copyright span {
      color: #888;
      display: block;
    }

    .js-footer .container .js-social-media {
      display: flex;
      justify-content: center;
    }

    .js-footer .container .js-social-media li {
      list-style: none;
      margin: auto 1.5rem;
    }

    .js-footer .container .js-social-media li a img {
      width: 2rem;
      -webkit-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -moz-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -o-transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      transition: .4s cubic-bezier(0.165, 0.84, 0.44, 1);
      -webkit-filter: grayscale(100%);
      -moz-filter: grayscale(100%);
      -o-filter: grayscale(100%);
      filter: grayscale(100%);
    }

    .js-footer .container .js-social-media li a img:hover {
      -webkit-transform: scale(1.1);
      -moz-transform: scale(1.1);
      -o-transform: scale(1.1);
      transform: scale(1.1);
    }
  }
</style>