<script>
  export let index;
</script>


<div class="p5">
    {#if index > 3}
      <div class="title">Encrypt Step 1: Plaintext, table and keyword</div>
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
      <div class="plain">Plaintext: THIS IS A FUN EXAMPLE</div>
      <div class="keyword">Keyword: 12,6,18,15,4,1,3,16,10,8,19,14,11,7,9,2,5,17,20,13</div>
      <div class="w1">The first step of encryption involves preparing the plaintext, the ADFGVX table, and the keyword. In this encryption tutorial, we will use "THIS IS A FUN EXAMPLE" as our plaintext and the ADFGVX table used by the German military along with a randomly chosen keyword.</div>
    {/if}
</div>


<style>  
  .p5 {
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
    left: 19%;
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

  @keyframes fadeInRight {
    from {
      opacity: 0;
      transform: translateX(2.278vh);
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
    left: 50%;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
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

  .keyword {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 85%;
    left: 50%;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 3s;
  }

  .plain {
     font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 75%;
    left: 50%;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 3s;
  }

  .w1 {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 2s;
  }


</style>
