<template>
  <div>

    <!-- How We Work -->
    <section id="how-js-work">
      <div class="container">
        <div class="js-section-header">
          <h1>How We Work</h1>
        </div>

        <div class="js-section-body">
          <main>
            <p>
              <span>Rencanakan</span>
              <br>
              Rencanakan project sampai matang dan siap diimplementasi.
            </p>
            <p>
              <span>Implementasi</span>
              <br>
              Hasil matang yang sudah direncanakan langsung di implementasikan.
            </p>
            <p>
              <span>Testing / Recheck</span>
              <br>
              Hasil yang sudah di implementasikan harus di check kembali agar tidak terjadi kesalahan.
            </p>
            <p>
              <span>Deploy dan Testing</span>
              <br>
              Ketika aplikasi sudah jadi, test lagi dan analisis apa yang kurang. Ulangi dari nomor 1.
            </p>
          </main>
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

