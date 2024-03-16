<script>
  export let index;
  let hoverW1 = false;
  let hoverW2 = false;
  let hoverW3 = false;
  let hoverW4 = false;
</script>


<div class="p4">
    {#if index > 2}
      <div class="title">The ADFGVX table & keyword</div>
      <table class="grid">
          <tr>
              <th class:highlight={hoverW1 || hoverW2}></th>
              <th class:highlight={hoverW1 || hoverW2}>A</th>
              <th class:highlight={hoverW1 || hoverW2}>D</th>
              <th class:highlight={hoverW1 || hoverW2}>F</th>
              <th class:highlight={hoverW1 || hoverW2}>G</th>
              <th class:highlight={hoverW1 || hoverW2}>V</th>
              <th class:highlight={hoverW1 || hoverW2}>X</th>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>A</th>
              <td class:highlight={hoverW1 || hoverW3}>C</td>
              <td class:highlight={hoverW1 || hoverW3}>O</td>
              <td class:highlight={hoverW1 || hoverW3}>8</td>
              <td class:highlight={hoverW1 || hoverW3}>X</td>
              <td class:highlight={hoverW1 || hoverW3}>F</td>
              <td class:highlight={hoverW1 || hoverW3}>4</td>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>D</th>
              <td class:highlight={hoverW1 || hoverW3}>M</td>
              <td class:highlight={hoverW1 || hoverW3}>K</td>
              <td class:highlight={hoverW1 || hoverW3}>3</td>
              <td class:highlight={hoverW1 || hoverW3}>A</td>
              <td class:highlight={hoverW1 || hoverW3}>Z</td>
              <td class:highlight={hoverW1 || hoverW3}>9</td>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>F</th>
              <td class:highlight={hoverW1 || hoverW3}>N</td>
              <td class:highlight={hoverW1 || hoverW3}>W</td>
              <td class:highlight={hoverW1 || hoverW3}>L</td>
              <td class:highlight={hoverW1 || hoverW3}>0</td>
              <td class:highlight={hoverW1 || hoverW3}>J</td>
              <td class:highlight={hoverW1 || hoverW3}>D</td>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>G</th>
              <td class:highlight={hoverW1 || hoverW3}>5</td>
              <td class:highlight={hoverW1 || hoverW3}>S</td>
              <td class:highlight={hoverW1 || hoverW3}>I</td>
              <td class:highlight={hoverW1 || hoverW3}>Y</td>
              <td class:highlight={hoverW1 || hoverW3}>H</td>
              <td class:highlight={hoverW1 || hoverW3}>U</td>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>V</th>
              <td class:highlight={hoverW1 || hoverW3}>P</td>
              <td class:highlight={hoverW1 || hoverW3}>1</td>
              <td class:highlight={hoverW1 || hoverW3}>V</td>
              <td class:highlight={hoverW1 || hoverW3}>B</td>
              <td class:highlight={hoverW1 || hoverW3}>6</td>
              <td class:highlight={hoverW1 || hoverW3}>R</td>
          </tr>
          <tr>
              <th class:highlight={hoverW1 || hoverW2}>X</th>
              <td class:highlight={hoverW1 || hoverW3}>E</td>
              <td class:highlight={hoverW1 || hoverW3}>Q</td>
              <td class:highlight={hoverW1 || hoverW3}>7</td>
              <td class:highlight={hoverW1 || hoverW3}>T</td>
              <td class:highlight={hoverW1 || hoverW3}>2</td>
              <td class:highlight={hoverW1 || hoverW3}>G</td>
          </tr>
      </table>
      <div class="keyword" class:highlight={hoverW1 || hoverW4}>Keyword: 12,6,18,15,4,1,3,16,10,8,19,14,11,7,9,2,5,17,20,13</div>
      <div class="w1" on:mouseover={() => hoverW1 = true} on:mouseout={() => hoverW1 = false} class:highlight={hoverW1}> The ADFGVX table and keyword are two essential elements for both encrypting and decrypting the ADFGVX cipher. The table on the left was used by the German army in 1918.</div>
      <div class="w2" on:mouseover={() => hoverW2 = true} on:mouseout={() => hoverW2 = false} class:highlight={hoverW2}>The ADFGVX table is a 6x6 grid formed by the six letters A, D, F, G, V, and X. Its content includes the 26 English letters plus the digits 0 through 9.</div>
      <div class="w3" on:mouseover={() => hoverW3 = true} on:mouseout={() => hoverW3 = false} class:highlight={hoverW3}> The contents of the table are randomly generated.</div>
      <div class="w4" on:mouseover={() => hoverW4 = true} on:mouseout={() => hoverW4 = false} class:highlight={hoverW4}> In the ADFGVX cipher, there are two types of keywords. The first type is a sequence of numbers, while the second type is a single word. In this tutorial, we will focus on the numerical keyword, which consists of a random sequence of numbers from 1 to n, where n is an even number.</div>
    {/if}
</div>

<style> 
  .p4 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
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
    top: 25%;
    left: 15%;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 2s;
  }

  .grid th, .grid td {
    border: 0.11vh solid white;
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
    left: 6%;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 2s;
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

  .w1 {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 21%;
    left: 57%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 3s;
  }

  .w2 {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 39%;
    left: 57%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 4s;
  }

  .w3 {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 56%;
    left: 57%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 5s;
  }

  .w4 {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 66%;
    left: 57%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 6s;
  }

  .highlight {
    color: orange;
  }
  
  .th-color, .td-color, .keyword-color {
    transition: color 0.3s ease;
  }

  .w1-color, .w2-color, .w3-color, .w4-color {
    transition: color 0.3s ease;
  }

</style>

