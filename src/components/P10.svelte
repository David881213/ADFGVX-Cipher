<script>
  export let index;

  let hoverW3 = false;
</script>


<div class="p10">
    {#if index > 8}
      <div class="title">Encrypt Step 3: Transposition Using a Keyword (1)</div>
      <div class="w1">The third step of encryption is Transposition Using a Keyword. Before transposition, we need to preprocess the substituted plaintext. First, we need to find out the keyword's total length. </div>
      <div class="keyword">Keyword: 12,6,18,15,4,1,3,16,10,8,19,14,11,7,9,2,5,17,20,13</div>
      <div class="len"> Length of Keyword = 20</div>
      <div class="w2">Then, we arrange the substituted plaintext in rows of 10 letters each.</div>
      <div class="spt">Substituted plaintext: XGGVGFGDGFGDDGAVGXFAXAAGDGDAVAFFXA</div>
      <table class="grid">
          <tr>
              <td>X</td>
              <td>G</td>
              <td>G</td>
              <td>V</td>
              <td>G</td>
              <td>F</td>
              <td>G</td>
              <td>D</td>
              <td>G</td>
              <td>F</td>
              <td>G</td>
              <td>D</td>
              <td>D</td>
              <td>G</td>
              <td>A</td>
              <td>V</td>
              <td>G</td>
              <td>X</td>
              <td>F</td>
              <td>A</td>
          </tr>
          <tr>
              <td>X</td>
              <td>A</td>
              <td>A</td>
              <td>G</td>
              <td>D</td>
              <td>G</td>
              <td>D</td>
              <td>A</td>
              <td>V</td>
              <td>A</td>
              <td>F</td>
              <td>F</td>
              <td>X</td>
              <td>A</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
              <td class="hidden" class:highlight={hoverW3}>X</td>
          </tr>
      </table>
      <div class="w3" on:mouseover={() => hoverW3 = true} on:mouseout={() => hoverW3 = false} class:highlight={hoverW3}>Finally, we fill any remaining spaces with 'X'.</div>
    {/if}
</div>s


<style>  
  .p10 {
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

  .circle1 {
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 2.8s;
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

  .grid {
    border-collapse: collapse;
    color: white;
    position: absolute;
    top: 59%;
    left: 15%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 5.1s;
  }

  .grid td {
    border: 1px solid white;
    width: 60px;  /* 或根据需要调整大小 */
    height: 60px; /* 或根据需要调整大小 */
    text-align: center;
    vertical-align: middle;
  }


  .grid td {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: normal;
  }

  .keyword {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 31%;
    left: 15%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 2.2s;
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

  .len {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    margin: 0;
    position: absolute;
    top: 30.5%;
    left: 67%;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 3.3s;
  }

  .w2 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 40%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 3.9s;
  }

  .spt {
    font-size: 28px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 50%;
    left: 15%;
    text-align: left;
    opacity: 0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 4.5s;
  }

  .w3 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 1400px;
    margin: 0;
    position: absolute;
    top: 80%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 5.7s;
  }

  @keyframes fadeInX {
    0% { opacity: 0; }
    100% { opacity: 1; }
  }

  .hidden {
    opacity: 0;
    animation: fadeInX 0.5s ease-out forwards;
    animation-delay: 6.3s; /* 延迟动画直到其他内容加载完成 */
  }

  .highlight {
    color: orange;
  }
  
  .w3, .hidden {
    transition: color 0.3s ease;
  }

</style>
