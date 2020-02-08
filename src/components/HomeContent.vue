<template>
  <div>

    <!-- About -->
    <section id="about-js-section">
      <div class="container">
        <div class="row">
          <div class="column column-50 column-left">
            <h1>About Us</h1>
            <p>Joy Studio is a group that is enthusiastic about making software. Joy Studio is currently focusing on the website and going into the mobile world (Android / IOS) in the future.
            </p>
          </div>
          <div class="column column-50 column-right">
            <img src="@/assets/images/logo.png" alt="">
          </div>
        </div>
      </div>
    </section>

    <section id="js-services-section">
      <div class="container">
        <div class="js-services-header">
          <h1>Our Service</h1>
        </div>

        <div class="js-services-body">
          <div class="row">
            <div class="column column-50 column-left">
              <div class="card">
                <img src="@/assets/images/web-development.svg" alt="" srcset="">

                <span class="js-service">
                  Web Development
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- How We Work -->
    <section id="how-js-work">
      <div class="container">
        <div class="js-section-header">
          <h1>How We Work</h1>
        </div>

        <div class="js-section-body">
          <main>
            <p>
              <span>Plan It</span>
              <br>
              Plan the project until it is done and ready to be implemented.
            </p>
            <p>
              <span>Implementation</span>
              <br>
              Mature results that have been planned are immediately implemented.
            </p>
            <p>
              <span>Testing / Recheck</span>
              <br>
              The results that have been implemented must be checked again so that no errors occur.
            </p>
            <p>
              <span>Deploy and Testing</span>
              <br>
              When the application is ready, test again and analyze what is lacking. Repeat from number 1.
            </p>
          </main>
        </div>
      </div>
    </section>

    <!-- Portfolio section -->
    <section id="js-portfolio-section">
      <div class="container">
        <div class="js-portfolio-header">
          <h1>Our Work</h1>
        </div>

        <div class="js-portfolio-body">
          <div class="row">
            <div class="column column-100">
              <div class="card">
                <div class="row">
                  <div class="column column-50 column-left">
                    <span class="portfolio-name">
                      Operational Dashboard Company
                    </span>
                  </div>
                  <div class="column column-50 column-right">
                    <img src="@/assets/images/Portfolio/OperationalApp.png" alt="" srcset="">
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Our Expertise -->
    <section id="js-technology-section">
      <div class="container">
        <div class="js-tech-header">
          <h1>Our Expertise</h1>
        </div>

        <div class="js-tech-body">
          <div class="row">
            <div class="column">
              <img src="@/assets/images/web-technology/reactjs.png" alt="" srcset="">
            </div>
            <div class="column">
              <img src="@/assets/images/web-technology/vue.png" alt="" srcset="">
            </div>
            <div class="column">
              <img src="@/assets/images/web-technology/expressjs.png" alt="" srcset="">
            </div>
          </div>
        </div>
      </div>
    </section>

  </div>
</template>

<style lang="scss" scoped>
  //Text Styles 
  $font-poppins: 'Poppins', sans-serif;

  //Colors
  $black: #34435E;
  $white: #ffffff;
  $primaryColor: #1DD1A1;

  * {
    font-family: $font-poppins;
  }

  #how-js-work {
    width: 100%;

    .js-section-header {
      margin: 50px auto;
    
      h1 {
        color: $primaryColor;
        font-weight: bold;
      }
    }

    .js-section-body {
      main {
        min-width: 300px;
        max-width: 500px;
        margin: auto;
      }

      span {
        font-weight: bold;
        color: $primaryColor;
        font-size: 2rem;
      }

      p {
        font-size: 1em;
        line-height: 1.75em;
        border-top: 3px solid;
        border-image: linear-gradient(to right, #0D5F4A 0%, #18B188 100%);
        border-image-slice: 1;
        border-width: 3px;
        margin: 0;
        padding: 40px;
        counter-increment: section;
        position: relative;
        color: $black;
        
        //numbers
        &:before {
          content: counter(section);
          position: absolute;
          border-radius: 50%;
          padding: 20px;
          height: 1.25em;
          width: 1.25em;
          background-color: $black;
          text-align: center;
          line-height: 0.2rem;
          color: $white;
          font-size: 1em;
        }
      }
      //odd number borders
      p:nth-child(odd) {
        border-right: 3px solid;
        padding-left: 0;
        
        &:before {
          left: 100%; 
          margin-left: -20px;
        }
      }
      //even number borders
      p:nth-child(even) {
        border-left: 3px solid;
        padding-right: 0;
        
        &:before {
          right: 100%; 
          margin-right: -20px;
        }
      }
      //handle first and last
      p:first-child {
        border-top: 0;
        border-top-right-radius:0;
        border-top-left-radius:0;
      }
      p:last-child {
        border-bottom-right-radius:0;
        border-bottom-left-radius:0;
      }
    }
  }
</style>

