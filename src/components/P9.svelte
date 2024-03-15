<script>
  export let index;
</script>


<div class="p9">
    {#if index > 7}
      <svg width=100% height=100vh>
        <circle class="circlet-1" cx=54.75% cy=66.2% r="22" fill="orange" />
        <line class="linet-1" x1=54.7% y1=66.3% x2=40% y2=66.3% stroke="orange" stroke-width="2" />
        <circle class="circlet-2" cx=39.85% cy=66.2% r="22" fill="orange" />
        <line class="linet-2" x1=54.7% y1=66.2% x2=54.7% y2=24% stroke="orange" stroke-width="2" />
        <circle class="circlet-3" cx=54.75% cy=23.4% r="22" fill="orange" />

        <circle class="circleh-1" cx=58.45% cy=52% r="22" fill="lightblue" />
        <line class="lineh-1" x1=58.4% y1=52.1% x2=40% y2=52.1% stroke="lightblue" stroke-width="2" />
        <circle class="circleh-2" cx=39.85% cy=52% r="22" fill="lightblue" />
        <line class="lineh-2" x1=58.4% y1=52% x2=58.4% y2=24% stroke="lightblue" stroke-width="2" />
        <circle class="circleh-3" cx=58.45% cy=23.4% r="22" fill="lightblue" />
      </svg>
      <div class="title">Encrypt Step 2: Substitution</div>
      <table class="grid">
          <tr>
              <th></th>
              <th>A</th>
              <th>D</th>
              <th>F</th>
              <th>G</th>
              <th>V</th>
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
              <th>G</th>
              <td>5</td>
              <td>S</td>
              <td>I</td>
              <td>Y</td>
              <td>H</td>
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
              <th>X</th>
              <td>E</td>
              <td>Q</td>
              <td>7</td>
              <td>T</td>
              <td>2</td>
              <td>G</td>
          </tr>
      </table>
      <div class="plain">Before: THISISAFUNEXAMPLE</div>
      <div class="w1">The second step in encryption involves removing spaces and punctuation from the plaintext. Then, each letter in the plaintext is replaced with its corresponding coordinates in the table. For example, "T" corresponds to the coordinates "XG".</div>
      <!-- T -->
      <div class="t">T</div>
      <div class="arrow1">→</div>
      <div class="t-c">XG</div>
      <!-- H -->
      <div class="h">H</div>
      <div class="arrow2">→</div>
      <div class="h-c">GV</div>
      <div class="arrow3">→</div>
      <div class="after">After: XGGVGFGDGFGDDGAVGXFAXAAGDGDAVAFFXA</div>
      <!-- I -->
      <div class="i">I</div>
      <div class="arrow4">→</div>
      <div class="i-c">GF</div>
      <!-- S -->
      <div class="s">S</div>
      <div class="arrow5">→</div>
      <div class="s-c">GD</div>
      <!-- I2 -->
      <div class="i2">I</div>
      <div class="arrow6">→</div>
      <div class="i2-c">GF</div>
      <!-- S2 -->
      <div class="s2">S</div>
      <div class="arrow7">→</div>
      <div class="s2-c">GD</div>
      <!-- A -->
      <div class="a">A</div>
      <div class="arrow8">→</div>
      <div class="a-c">DG</div>
      <!-- F -->
      <div class="f">F</div>
      <div class="arrow17">→</div>
      <div class="f-c">AV</div>
      <!-- U -->
      <div class="u">U</div>
      <div class="arrow18">→</div>
      <div class="u-c">GX</div>
      <!-- N -->
      <div class="n">N</div>
      <div class="arrow9">→</div>
      <div class="n-c">FA</div>
      <!-- E -->
      <div class="e">E</div>
      <div class="arrow10">→</div>
      <div class="e-c">XA</div>
      <!-- X -->
      <div class="x">X</div>
      <div class="arrow11">→</div>
      <div class="x-c">AG</div>
      <!-- A2 -->
      <div class="a2">A</div>
      <div class="arrow12">→</div>
      <div class="a2-c">DG</div>
      <!-- M -->
      <div class="m">M</div>
      <div class="arrow13">→</div>
      <div class="m-c">DA</div>
      <!-- P -->
      <div class="p">P</div>
      <div class="arrow14">→</div>
      <div class="p-c">VA</div>
      <!-- L -->
      <div class="l">L</div>
      <div class="arrow15">→</div>
      <div class="l-c">FF</div>
      <!-- E2 -->
      <div class="e2">E</div>
      <div class="arrow16">→</div>
      <div class="e2-c">XA</div>
    {/if}
</div>


<style> 
  
  @keyframes drawLine {
    from {
      stroke-dashoffset: 100%;
    }
    to {
      stroke-dashoffset: 0%;
    }
  }
  .linet-1 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 4.8s;
  }

  .linet-2 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 5.4s;
  }

  .lineh-1 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 7.6s;
  }

  .lineh-2 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 8.2s;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .circlet-1 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 4.4s;
  }
  .circlet-2 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 5s;
  }
  .circlet-3 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 5.6s;
  }

  .circleh-1 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 7.2s;
  }
  .circleh-2 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 7.8s;
  }
  .circleh-3 {
    position: absolute;
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 8.4s;
  }

  .p9 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;      
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


  .title {
    font-size: 50px;
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
      transform: translateX(-20px);
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
    width: 60px;  /* 或根据需要调整大小 */
    height: 60px; /* 或根据需要调整大小 */
    text-align: center;
    vertical-align: middle;
  }

  .grid th {
    font-size: 28px;
    font-weight: bold;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  }

  .grid td {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: normal;
  }

  .plain {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 83%;
    left:8%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 10s;
  }

  .w1 {
    font-size: 32px;
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

  .arrow3 {
    font-size: 40px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 82%;
    left: 39%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 10.6s;
  }

  .after {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 83%;
    left:43%;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 11.2s;
  }

  .t {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.8s;
  }

  .arrow1 {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 24.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 6s;
  }

  .t-c {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 6.3s;
  }

  .h {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 6.6s;
  }

  .arrow2 {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 32.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 8.8s;
  }

  .h-c {
    font-size: 45px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 33%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.2s;
  }

  .i {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 70.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow4 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .i-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .s {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow5 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .s-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .i2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 70.5%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow6 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .i2-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .s2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow7 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .s2-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .a {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow8 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .a-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .f {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left: 70%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow17 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 64.5%;
    left: 73%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .f-c {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left: 77%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .u {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 25%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow18 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .u-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .n {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 30%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow9 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .n-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .e {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow10 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .e-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .x {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow11 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .x-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .a2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow12 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .a2-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .m {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow13 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .m-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .p {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 55%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow14 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .p-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .l {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow15 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .l-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .e2 {
    font-size: 35px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 65%;
    left: 83%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.3s ease-out forwards;
    animation-delay: 9.6s;
  }

  .arrow16 {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }

  .e2-c {
    font-size: 35px;
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
    animation-delay: 9.6s;
  }
</style>
