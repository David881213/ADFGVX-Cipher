<script>
  export let index;
</script>


<div class="p8">
    {#if index > 6}
      <div class="title">Encrypt Step 3: Transposition Using a Keyword (2)</div>
      <div class="w1">Assign numbers to each column according to the order of the keyword, then rearrange the columns in ascending order based on the assigned numbers.</div>
      <!-- key -->
      <div class="k0">Keyword: </div>
      <div class="k1">12</div>
      <div class="k2">6</div>
      <div class="k3">18</div>
      <div class="k4">15</div>
      <div class="k5">4</div>
      <div class="k6">1</div>
      <div class="k7">3</div>
      <div class="k8">16</div>
      <div class="k9">10</div>
      <div class="k10">8</div>
      <div class="k11">19</div>
      <div class="k12">14</div>
      <div class="k13">11</div>
      <div class="k14">7</div>
      <div class="k15">9</div>
      <div class="k16">2</div>
      <div class="k17">5</div>
      <div class="k18">17</div>
      <div class="k19">20</div>
      <div class="k20">13</div>
      <!-- stay -->
      <div class="a1">X X</div>
      <div class="a2">G A</div>
      <div class="a3">G A</div>
      <div class="a4">V G</div>
      <div class="a5">G D</div>
      <div class="a6">F G</div>
      <div class="a7">G D</div>
      <div class="a8">D A</div>
      <div class="a9">G V</div>
      <div class="a10">F A</div>
      <div class="a11">G F</div>
      <div class="a12">D F</div>
      <div class="a13">D X</div>
      <div class="a14">G A</div>
      <div class="a15">A X</div>
      <div class="a16">V X</div>
      <div class="a17">G X</div>
      <div class="a18">X X</div>
      <div class="a19">F X</div>
      <div class="a20">A X</div>
      <!-- key2 -->
      <div class="k0-2">Keyword: </div>
      <div class="k1-2">12</div>
      <div class="k2-2">6</div>
      <div class="k3-2">18</div>
      <div class="k4-2">15</div>
      <div class="k5-2">4</div>
      <div class="k6-2">1</div>
      <div class="k7-2">3</div>
      <div class="k8-2">16</div>
      <div class="k9-2">10</div>
      <div class="k10-2">8</div>
      <div class="k11-2">19</div>
      <div class="k12-2">14</div>
      <div class="k13-2">11</div>
      <div class="k14-2">7</div>
      <div class="k15-2">9</div>
      <div class="k16-2">2</div>
      <div class="k17-2">5</div>
      <div class="k18-2">17</div>
      <div class="k19-2">20</div>
      <div class="k20-2">13</div>
      <!-- go -->
      <div class="b1">X X</div>
      <div class="b2">G A</div>
      <div class="b3">G A</div>
      <div class="b4">V G</div>
      <div class="b5">G D</div>
      <div class="b6">F G</div>
      <div class="b7">G D</div>
      <div class="b8">D A</div>
      <div class="b9">G V</div>
      <div class="b10">F A</div>
      <div class="b11">G F</div>
      <div class="b12">D F</div>
      <div class="b13">D X</div>
      <div class="b14">G A</div>
      <div class="b15">A X</div>
      <div class="b16">V X</div>
      <div class="b17">G X</div>
      <div class="b18">X X</div>
      <div class="b19">F X</div>
      <div class="b20">A X</div>

      <div class="w2">Next, merge each column sequentially according to the order.</div>
      <div class="result">Ciphertext: FGVXGDGDGXGAGAFAAXGVDXXXAXDFVGDAXXGAGFFX</div>
    {/if}
</div>


<style>  
  .p8 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;      
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  @keyframes fadeInLeft {
    from {
      opacity: 0;
      transform: translateX(-20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  @keyframes fadeInRight {
    from {
      opacity: 0;
      transform: translateX(20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .title {
    font-size: 50px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 5%;
    left: 15%;
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 0.5s;
  }

  .w1 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 16%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.6s;
  }

  .w2 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 70%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 7s;
  }

  .result {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 80%;
    left: 20%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 7.6s;
  }

  /* stay ---------------------------------------------------------------------------------------------------------------------*/

  .a1 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 21%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 24%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a3 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 27%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a4 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 30%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a5 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 33%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a6 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 36%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a7 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 39%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a8 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 42%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a9 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 45%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a10 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 48%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a11 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 51%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a12 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 54%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a13 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 57%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a14 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 60%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a15 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 63%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a16 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 66%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a17 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 69%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a18 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 72%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a19 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 75%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  .a20 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 78%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
  }

  /* keyword-------------------------------------------------------------------------------------------------------------- */

  .k0 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 13%;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 2.8s;
  }

  .k1 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 20.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 24.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k3 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 26.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k4 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 29.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k5 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 33.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k6 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 36.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k7 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 39.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k8 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 41.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k9 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 44.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k10 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 48.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k11 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 50.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k12 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 53.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k13 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 56.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k14 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 60.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k15 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 63.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k16 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 66.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k17 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 69.3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k18 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 71.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k19 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 74.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  .k20 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 77.7%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.4s;
  }

  /* go ---------------------------------------------------------------------------------------------------------------------*/

  .b1 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 21%;
    opacity: 0;
    animation: moveb12 1s ease-out forwards;
    animation-delay: 4s;
  }

  .b2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 24%;
    opacity: 0;
    animation: moveb6 1s ease-out forwards;
    animation-delay: 4.1s;
  }

  .b3 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 27%;
    opacity: 0;
    animation: moveb18 1s ease-out forwards;
    animation-delay: 4.2s;
  }

  .b4 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 30%;
    opacity: 0;
    animation: moveb15 1s ease-out forwards;
    animation-delay: 4.3s;
  }

  .b5 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 33%;
    opacity: 0;
    animation: moveb4 1s ease-out forwards;
    animation-delay: 4.4s;
  }

  .b6 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 36%;
    opacity: 0;
    animation: moveb1 1s ease-out forwards;
    animation-delay: 4.5s;
  }

  .b7 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 39%;
    opacity: 0;
    animation: moveb3 1s ease-out forwards;
    animation-delay: 4.6s;
  }

  .b8 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 42%;
    opacity: 0;
    animation: moveb16 1s ease-out forwards;
    animation-delay: 4.7s;
  }

  .b9 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 45%;
    opacity: 0;
    animation: moveb10 1s ease-out forwards;
    animation-delay: 4.8s;
  }

  .b10 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 48%;
    opacity: 0;
    animation: moveb8 1s ease-out forwards;
    animation-delay: 4.9s;
  }

  .b11 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 51%;
    opacity: 0;
    animation: moveb19 1s ease-out forwards;
    animation-delay: 5s;
  }

  .b12 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 54%;
    opacity: 0;
    animation: moveb14 1s ease-out forwards;
    animation-delay: 5.1s;
  }

  .b13 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 57%;
    opacity: 0;
    animation: moveb11 1s ease-out forwards;
    animation-delay: 5.2s;
  }

  .b14 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 60%;
    opacity: 0;
    animation: moveb7 1s ease-out forwards;
    animation-delay: 5.3s;
  }

  .b15 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 63%;
    opacity: 0;
    animation: moveb9 1s ease-out forwards;
    animation-delay: 5.4s;
  }

  .b16 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 66%;
    opacity: 0;
    animation: moveb2 1s ease-out forwards;
    animation-delay: 5.5s;
  }

  .b17 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 69%;
    opacity: 0;
    animation: moveb5 1s ease-out forwards;
    animation-delay: 5.6s;
  }

  .b18 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 72%;
    opacity: 0;
    animation: moveb17 1s ease-out forwards;
    animation-delay: 5.7s;
  }

  .b19 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 75%;
    opacity: 0;
    animation: moveb20 1s ease-out forwards;
    animation-delay: 5.8s;
  }

  .b20 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 78%;
    opacity: 0;
    animation: moveb13 1s ease-out forwards;
    animation-delay: 5.9s;
  }

  /* keyword-------------------------------------------------------------------------------------------------------------- */

  .k1-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 20.7%;
    opacity: 0;
    animation: movek12 1s ease-out forwards;
    animation-delay: 4s;
  }

  .k2-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 24.3%;
    opacity: 0;
    animation: movek6 1s ease-out forwards;
    animation-delay: 4.1s;
  }

  .k3-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 26.7%;
    opacity: 0;
    animation: movek18 1s ease-out forwards;
    animation-delay: 4.2s;
  }

  .k4-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 29.7%;
    opacity: 0;
    animation: movek15 1s ease-out forwards;
    animation-delay: 4.3s;
  }

  .k5-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 33.3%;
    opacity: 0;
    animation: movek4 1s ease-out forwards;
    animation-delay: 4.4s;
  }

  .k6-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 36.3%;
    opacity: 0;
    animation: movek1 1s ease-out forwards;
    animation-delay: 4.5s;
  }

  .k7-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 39.3%;
    opacity: 0;
    animation: movek3 1s ease-out forwards;
    animation-delay: 4.6s;
  }

  .k8-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 41.7%;
    opacity: 0;
    animation: movek16 1s ease-out forwards;
    animation-delay: 4.7s;
  }

  .k9-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 44.7%;
    opacity: 0;
    animation: movek10 1s ease-out forwards;
    animation-delay: 4.8s;
  }

  .k10-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 48.3%;
    opacity: 0;
    animation: movek8 1s ease-out forwards;
    animation-delay: 4.9s;
  }

  .k11-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 50.7%;
    opacity: 0;
    animation: movek19 1s ease-out forwards;
    animation-delay: 5s;
  }

  .k12-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 53.7%;
    opacity: 0;
    animation: movek14 1s ease-out forwards;
    animation-delay: 5.1s;
  }

  .k13-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 56.7%;
    opacity: 0;
    animation: movek11 1s ease-out forwards;
    animation-delay: 5.2s;
  }

  .k14-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 60.3%;
    opacity: 0;
    animation: movek7 1s ease-out forwards;
    animation-delay: 5.3s;
  }

  .k15-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 63.3%;
    opacity: 0;
    animation: movek9 1s ease-out forwards;
    animation-delay: 5.4s;
  }

  .k16-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 66.3%;
    opacity: 0;
    animation: movek2 1s ease-out forwards;
    animation-delay: 5.5s;
  }

  .k17-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 69.3%;
    opacity: 0;
    animation: movek5 1s ease-out forwards;
    animation-delay: 5.6s;
  }

  .k18-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 71.7%;
    opacity: 0;
    animation: movek17 1s ease-out forwards;
    animation-delay: 5.7s;
  }

  .k19-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 74.7%;
    opacity: 0;
    animation: movek20 1s ease-out forwards;
    animation-delay: 5.8s;
  }

  .k20-2 {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    max-width: 20px;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 77.7%;
    opacity: 0;
    animation: movek13 1s ease-out forwards;
    animation-delay: 5.9s;
  }

  @keyframes moveb1 {
    from {
        top: 33%; 
        left: 36%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 21%; 
        opacity: 1;
    }
  }

  @keyframes moveb2 {
    from {
        top: 33%; 
        left: 66%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 24%; 
        opacity: 1;
    }
  }
  @keyframes moveb3 {
    from {
        top: 33%; 
        left: 39%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 27%; 
        opacity: 1;
    }
  }
  @keyframes moveb4 {
    from {
        top: 33%; 
        left: 33%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 30%; 
        opacity: 1;
    }
  }
  @keyframes moveb5 {
    from {
        top: 33%; 
        left: 69%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 33%; 
        opacity: 1;
    }
  }
  @keyframes moveb6 {
    from {
        top: 33%; 
        left: 24%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 36%; 
        opacity: 1;
    }
  }
  @keyframes moveb7 {
    from {
        top: 33%; 
        left: 60%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 39%; 
        opacity: 1;
    }
  }
  @keyframes moveb8 {
    from {
        top: 33%; 
        left: 48%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 42%; 
        opacity: 1;
    }
  }
  @keyframes moveb9 {
    from {
        top: 33%; 
        left: 63%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 45%; 
        opacity: 1;
    }
  }
  @keyframes moveb10 {
    from {
        top: 33%; 
        left: 45%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 48%; 
        opacity: 1;
    }
  }
  @keyframes moveb11 {
    from {
        top: 33%; 
        left: 57%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 51%; 
        opacity: 1;
    }
  }

  @keyframes moveb12 {
    from {
        top: 33%; 
        left: 21%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 54%; 
        opacity: 1;
    }
  }
  @keyframes moveb13 {
    from {
        top: 33%; 
        left: 78%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 57%; 
        opacity: 1;
    }
  }
  @keyframes moveb14 {
    from {
        top: 33%; 
        left: 54%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 60%; 
        opacity: 1;
    }
  }
  @keyframes moveb15 {
    from {
        top: 33%; 
        left: 30%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 63%; 
        opacity: 1;
    }
  }
  @keyframes moveb16 {
    from {
        top: 33%; 
        left: 42%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 66%; 
        opacity: 1;
    }
  }
  @keyframes moveb17 {
    from {
        top: 33%; 
        left: 72%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 69%; 
        opacity: 1;
    }
  }
  @keyframes moveb18 {
    from {
        top: 33%; 
        left: 27%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 72%; 
        opacity: 1;
    }
  }
  @keyframes moveb19 {
    from {
        top: 33%; 
        left: 51%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 75%; 
        opacity: 1;
    }
  }
  @keyframes moveb20 {
    from {
        top: 33%; 
        left: 75%; 
        opacity: 0;
    }
    to {
        top: 53%; 
        left: 78%; 
        opacity: 1;
    }
  }

  /*keya-------------------------------------------------------------------------------------------------------------------*/

  @keyframes movek1 {
    from {
        top: 28%; 
        left: 36.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 21.3%; 
        opacity: 1;
    }
  }

  @keyframes movek2 {
    from {
        top: 28%; 
        left: 66.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 24.3%; 
        opacity: 1;
    }
  }
  @keyframes movek3 {
    from {
        top: 28%; 
        left: 39.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 27.3%; 
        opacity: 1;
    }
  }
  @keyframes movek4 {
    from {
        top: 28%; 
        left: 33.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 30.3%; 
        opacity: 1;
    }
  }
  @keyframes movek5 {
    from {
        top: 28%; 
        left: 69.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 33.3%; 
        opacity: 1;
    }
  }
  @keyframes movek6 {
    from {
        top: 28%; 
        left: 24.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 36.3%; 
        opacity: 1;
    }
  }
  @keyframes movek7 {
    from {
        top: 28%; 
        left: 60.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 39.3%; 
        opacity: 1;
    }
  }
  @keyframes movek8 {
    from {
        top: 28%; 
        left: 48.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 42.3%; 
        opacity: 1;
    }
  }
  @keyframes movek9 {
    from {
        top: 28%; 
        left: 63.3%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 45.3%; 
        opacity: 1;
    }
  }
  @keyframes movek10 {
    from {
        top: 28%; 
        left: 44.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 47.7%; 
        opacity: 1;
    }
  }
  @keyframes movek11 {
    from {
        top: 28%; 
        left: 56.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 50.7%; 
        opacity: 1;
    }
  }

  @keyframes movek12 {
    from {
        top: 28%; 
        left: 20.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 53.7%; 
        opacity: 1;
    }
  }
  @keyframes movek13 {
    from {
        top: 28%; 
        left: 77.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 56.7%; 
        opacity: 1;
    }
  }
  @keyframes movek14 {
    from {
        top: 28%; 
        left: 53.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 59.7%; 
        opacity: 1;
    }
  }
  @keyframes movek15 {
    from {
        top: 28%; 
        left: 29.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 62.7%; 
        opacity: 1;
    }
  }
  @keyframes movek16 {
    from {
        top: 28%; 
        left: 41.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 65.7%; 
        opacity: 1;
    }
  }
  @keyframes movek17 {
    from {
        top: 28%; 
        left: 71.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 68.7%; 
        opacity: 1;
    }
  }
  @keyframes movek18 {
    from {
        top: 28%; 
        left: 26.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 71.7%; 
        opacity: 1;
    }
  }
  @keyframes movek19 {
    from {
        top: 28%; 
        left: 50.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 74.7%; 
        opacity: 1;
    }
  }
  @keyframes movek20 {
    from {
        top: 28%; 
        left: 74.7%; 
        opacity: 0;
    }
    to {
        top: 48%; 
        left: 77.7%; 
        opacity: 1;
    }
  }
</style>
