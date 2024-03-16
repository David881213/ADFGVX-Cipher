<script>
  export let index;
</script>

<div class="page-container">

  {#if index <= 9}
    <div class="background2" ></div>
  {/if}
  {#if index > 9}

    <div class="background" ></div>
    <div class="title">
        <p> Breaker of ADFGVX System </p>
    </div>
    <div class="decrypt">
        <p> Although the ADFGVX Cipher appears complex, it was actually decrypted during WWI.</p>
    </div>
    <div class="breaker">
        <p> The ADFGVX system was broke by Geogers-Jean Painvin</p>
    </div>
    <div class="breaker2">
        <p> One of the greatest cryptanalysis of Frence</p>
    </div>
    <div class="breaker3">
        <p> Geogers-Jean Painvin (1886-1980)</p>
    </div>
    <div class="Painvin">
        <img src="painv4.jpg" alt="Painvin">
    </div>
  {/if}

</div>

<style>

  @keyframes fadeOut {
    from { opacity: 1; }
    to { opacity: 0.1; }
  }

  .background {
    background: black;
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 1;
    animation: fadeOut 0.3s ease-out forwards;
    animation-delay: 0.5s;
  }

  .background2 {
    background: black;
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 2;
  }

  .page-container {
    position: relative;
    width: 100%;
    height: 100vh;
    margin: 0;
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
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 0vh;
    font-size: 5.695vh;
    left: 0%;
    margin: 0;
    white-space: nowrap;
    opacity:0;
    animation: fadeInUp 0.3s ease-out forwards;
    animation-delay: 0.5s;
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

  .decrypt {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 50%;
    top: 20vh;
    font-size: 4.556vh;
    left: 44%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }

  .breaker {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 50%;
    top: 45vh;
    font-size: 4.556vh;
    left: 44%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }
  .breaker2 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 50%;
    top: 65vh;
    font-size: 4.556vh;
    left: 44%;
    white-space: nowrap;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 3.3s;
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

  .breaker3 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 78vh;
    font-size: 2.278vh;
    left: -22%;
    white-space: nowrap;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.3s;
  }
  .Painvin{
    position: absolute;
    top: 25vh;
    left: 20%;
    width : 10vw;
    height: 10vh;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.3s;
  }

  </style>