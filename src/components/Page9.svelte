<script>
  export let index;
</script>

<div class="p9">
  {#if index > 7}
      <div class="title">Encrypt Step 4: 5-Gram</div>
      <div class="w1">The final step of encryption is to convert the entire ciphertext into 5-grams.</div>
      <div class="w2">Ciphertext: FGVXGDGDGXGAGAFAAXGVDXXXAXDFVGDAXXGAGFFX</div>
      <div class="five">5-Gram: FGVXG  DGDGX  GAGAF  AAXGV  DXXXA  XDFVG  DAXXG  AGFFX</div>
      <div class="w3">Finally, we obtain the ciphertext:</div>
      <div class="w4">"FGVXG  DGDGX  GAGAF  AAXGV  DXXXA  XDFVG  DAXXG  AGFFX"</div>
  {/if}
</div>

<style> 
  .p9 {
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
    left: 35%;
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

  .w1 {
    font-size: 3.645vh;
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

  .w2 {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 20%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 2.4s;
  }

  .five {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 20%;
    text-align: left;
    opacity: 0;
    animation: fadeInRight 0.7s ease-out forwards;
    animation-delay: 3.2s;
  }

  .w3 {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 4s;
  }

  .w4 {
    font-size: 4.328vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: orange;
    margin: 0;
    position: absolute;
    top: 70%;
    left: 15%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 4.8s;
  }


</style>

