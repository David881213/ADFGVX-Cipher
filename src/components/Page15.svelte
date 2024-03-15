<script>
  export let index;
  let hoverW3 = false;
</script>


<div class="p15">
  {#if index > 13}
      <div class="title">Decrypt Step 2: Remove 5-Gram & reconstruct the cipher columns</div>
      <div class="w1">The second step of decryption is to remove the space in entire ciphertext.</div>
      <div class="cols">Then, similar as encrypt, we arrange the ciphertext in rows of 20 letters each, which the length of the keyword. </div>
      <div class="w2">Ciphertext: FGVXGDGDGXGAGAFAAXGVDXXXAXDFVGDAXXGAGFFX</div>
      <div class="five">5-Gram: FGVXG  DGDGX  GAGAF  AAXGV  DXXXA  XDFVG  DAXXG  AGFFX</div>
      <table class="grid">
          <tr>
              <td>F</td>
              <td>G</td>
              <td>V</td>
              <td>X</td>
              <td>G</td>
              <td>D</td>
              <td>G</td>
              <td>D</td>
              <td>G</td>
              <td>X</td>
              <td>G</td>
              <td>A</td>
              <td>G</td>
              <td>A</td>
              <td>F</td>
              <td>A</td>
              <td>A</td>
              <td>X</td>
              <td>G</td>
              <td>V</td>
          </tr>
          <tr>
              <td>D</td>
              <td>X</td>
              <td>X</td>
              <td>X</td>
              <td>A</td>
              <td>X</td>
              <td>D</td>
              <td>F</td>
              <td>V</td>
              <td>G</td>
              <td>D</td>
              <td>A</td>
              <td>X</td>
              <td>X</td>
              <td class="hidden" class:highlight={hoverW3}>G</td>
              <td class="hidden" class:highlight={hoverW3}>A</td>
              <td class="hidden" class:highlight={hoverW3}>G</td>
              <td class="hidden" class:highlight={hoverW3}>F</td>
              <td class="hidden" class:highlight={hoverW3}>F</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
          </tr>
      </table>
  {/if}
</div>

<style> 
  .p15 {
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
    left: 3%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 0.5s;
    white-space: nowrap;
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

  .w1 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 21%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 1.6s;
  }

  .five {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 31%;
    left: 14%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 2.4s;
  }

  .w2 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 41%;
    left: 14%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 3.2s;
  }

  

  .cols {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 51%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 4s;
  }

  .grid {
    border-collapse: collapse;
    color: white;
    position: absolute;
    top: 64%;
    left: 15%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 5.1s;
  }

  .grid td {
    border: 1px solid white;
    width: 60px;
    height: 60px;
    text-align: center;
    vertical-align: middle;
  }


  .grid td {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: normal;
  }



</style>

