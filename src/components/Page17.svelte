<script>
  export let index;
</script>


<div class="p17">
    {#if index > 15}
      <div class="title">Decrypt Step 4: Substitution</div>
      <table class="grid">
          <tr>
              <th></th>
              <th>A</th>
              <th>D</th>
              <th>F</th>
              <th class="highlight-t2">G</th>
              <th class="highlight-h2">V</th>
              <th>X</th>
          </tr>
          <tr>
              <th>A</th>
              <td>C</td>
              <td>O</td>
              <td>8</td>
              <td>X</td>
              <td>F</td>
              <td>4</td>
          </tr>
          <tr>
              <th>D</th>
              <td>M</td>
              <td>K</td>
              <td>3</td>
              <td>A</td>
              <td>Z</td>
              <td>9</td>
          </tr>
          <tr>
              <th>F</th>
              <td>N</td>
              <td>W</td>
              <td>L</td>
              <td>0</td>
              <td>J</td>
              <td>D</td>
          </tr>
          <tr>
              <th class="highlight-h1">G</th>
              <td>5</td>
              <td>S</td>
              <td>I</td>
              <td>Y</td>
              <td class="highlight-h3">H</td>
              <td>U</td>
          </tr>
          <tr>
              <th>V</th>
              <td>P</td>
              <td>1</td>
              <td>V</td>
              <td>B</td>
              <td>6</td>
              <td>R</td>
          </tr>
          <tr>
              <th class="highlight-t1">X</th>
              <td>E</td>
              <td>Q</td>
              <td>7</td>
              <td class="highlight-t3">T</td>
              <td>2</td>
              <td>G</td>
          </tr>
      </table>
      <div class="all3">All 3 pairs of XX:</div>
      <div class="plain">Before: XGGVGFGDGFGDDGAVGXFAXAAGDGDAVAFFXAXXXXXX</div>
      <div class="w1">The fourth step in decryption each pair of cipher in the ciphertext is replaced with their corresponding letter in the table. For example, " XG " corresponds to the coordinates "T".</div>
      <!-- T -->
      <div class="t">XG</div>
      <div class="arrow1">→</div>
      <div class="t-c">T</div>
      <!-- H -->
      <div class="h">GV</div>
      <div class="arrow2">→</div>
      <div class="h-c">H</div>
      <div class="arrow3">→</div>
      <div class="after">After: THISISAFUNEXAMPLEGGG</div>
      <!-- I -->
      <div class="i">GF</div>
      <div class="arrow4">→</div>
      <div class="i-c">I</div>
      <!-- S -->
      <div class="s">GD</div>
      <div class="arrow5">→</div>
      <div class="s-c">S</div>
      <!-- I2 -->
      <div class="i2">GF</div>
      <div class="arrow6">→</div>
      <div class="i2-c">I</div>
      <!-- S2 -->
      <div class="s2">GD</div>
      <div class="arrow7">→</div>
      <div class="s2-c">S</div>
      <!-- A -->
      <div class="a">DG</div>
      <div class="arrow8">→</div>
      <div class="a-c">A</div>
      <!-- F -->
      <div class="f">AV</div>
      <div class="arrow17">→</div>
      <div class="f-c">F</div>
      <!-- U -->
      <div class="u">GX</div>
      <div class="arrow18">→</div>
      <div class="u-c">U</div>
      <!-- N -->
      <div class="n">FA</div>
      <div class="arrow9">→</div>
      <div class="n-c">N</div>
      <!-- E -->
      <div class="e">XA</div>
      <div class="arrow10">→</div>
      <div class="e-c">E</div>
      <!-- X -->
      <div class="x">AG</div>
      <div class="arrow11">→</div>
      <div class="x-c">X</div>
      <!-- A2 -->
      <div class="a2">DG</div>
      <div class="arrow12">→</div>
      <div class="a2-c">A</div>
      <!-- M -->
      <div class="m">DA</div>
      <div class="arrow13">→</div>
      <div class="m-c">M</div>
      <!-- P -->
      <div class="p">VA</div>
      <div class="arrow14">→</div>
      <div class="p-c">P</div>
      <!-- L -->
      <div class="l">FF</div>
      <div class="arrow15">→</div>
      <div class="l-c">L</div>
      <!-- E2 -->
      <div class="e2">XA</div>
      <div class="arrow16">→</div>
      <div class="e2-c">E</div>
      <!-- G -->
      <div class="g">XX</div>
      <div class="arrowg">→</div>
      <div class="g-c">G</div>
    {/if}
</div>


<style> 

  @keyframes highlightAnimation {
    from {
      font-size: 3.189vh;
      color: white;
    }
    to {
      font-size: 4.5vh;
      color: orange;
    }
  }

  @keyframes highlightAnimation2 {
    from {
      font-size: 3.189vh;
      color: white;
    }
    to {
      font-size: 4.5vh;
      color: red;
    }
  }
  
  @keyframes drawLine {
    from {
      stroke-dashoffset: 100%;
    }
    to {
      stroke-dashoffset: 0%;
    }
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .p17 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;      
  }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(2.278vh);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }


  .title {
    font-size: 5.695vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 5%;
    left: 30%;
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 0.5s;
  }

  @keyframes fadeInLeft {
    from {
      opacity: 0;
      transform: translateX(-2.278vh);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .grid {
    border-collapse: collapse;
    color: white;
    position: absolute;
    top: 20%;
    left: 38%;
    opacity: 0;
    animation: fadeInUp 0.7s ease-out forwards;
    animation-delay: 3s;
  }

  .grid th, .grid td {
    border: 1px solid white;
    width: 6.834vh; 
    height: 6.834vh; 
    text-align: center;
    vertical-align: middle;
  }

  .grid th {
    font-size: 3.189vh;
    font-weight: bold;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  }

  .grid td {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: normal;
  }

  .grid .highlight-t1 {
    animation: highlightAnimation 0.3s ease-out forwards;
    animation-delay: 4.4s;
  }

  .grid .highlight-t2 {
    animation: highlightAnimation 0.3s ease-out forwards;
    animation-delay: 4.8s; 
  }

  .grid .highlight-t3 {
    animation: highlightAnimation 0.3s ease-out forwards;
    animation-delay: 5.2s;
  }

  .grid .highlight-h1 {
    animation: highlightAnimation2 0.3s ease-out forwards;
    animation-delay: 7.2s;
  }

  .grid .highlight-h2 {
    animation: highlightAnimation2 0.3s ease-out forwards;
    animation-delay: 7.6s;
  }

  .grid .highlight-h3 {
    animation: highlightAnimation2 0.3s ease-out forwards;
    animation-delay: 8s;
  }

  .w1 {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 450px;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 8%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 2s;
  }

  .t {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    margin: 0;
    position: absolute;
    top: 20%;
    left: 69%;
    text-align: left;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.8s;
  }

  .arrow1 {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    margin: 0;
    position: absolute;
    top: 19.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 4.8s;
  }

  .t-c {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    margin: 0;
    position: absolute;
    top: 20%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 5.8s;
  }

  .h {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: red;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 69%;
    text-align: left;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 6.8s;
  }

  .arrow2 {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: red;
    margin: 0;
    position: absolute;
    top: 27.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 7.8s;
  }

  .h-c {
    font-size: 5.125vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: red;
    margin: 0;
    position: absolute;
    top: 28%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 8.8s;
  }

  .i {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow4 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 34.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .i-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .s {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow5 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 39.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .s-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .i2 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow6 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 44.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .i2-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .s2 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow7 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 49.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .s2-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .a {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow8 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 54.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .a-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .f {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 69.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow17 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 59.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .f-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .u {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 20%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow18 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 19.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .u-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 20%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .n {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow9 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 24.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .n-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .e {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 30%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow10 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 29.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .e-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 30%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .x {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow11 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 34.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .x-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .a2 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow12 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 39.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .a2-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .m {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow13 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 44.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .m-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .p {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow14 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 49.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .p-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .l {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow15 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 54.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .l-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .e2 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .arrow16 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 59.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }

  .e2-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.8s;
  }
  .g {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left: 82.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 11.8s;
  }

  .arrowg {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 64.5%;
    left: 86%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 11.8s;
  }

  .g-c {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left: 90%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 11.8s;
  }
  .all3 {
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left:66%;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 10.8s;
  }

  .plain {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 83%;
    left:4%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 12.8s;
  }

  .arrow3 {
    font-size: 4.556vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 82%;
    left: 63.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 13.8s;
  }

  .after {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 83%;
    left:67%;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 14.8s;
  }
</style>
