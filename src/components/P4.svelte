<script>
    export let index;
</script>


<div class="p4">
  {#if index > 2}
    <div class="title">
        <p> Breaker of ADFGVX System </p>
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
  .p4 {
    position: relative;
    background: transparent;
    width: 100vh;
    height: 100%;
    margin: 0;            
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
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 5vh;
    font-size: 50px;
    left: 55%;
    margin: 0;
    white-space: nowrap;
    opacity:0;
    animation: fadeInUp 0.3s ease-out forwards;
    animation-delay: 0.5s;
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

  .breaker {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 40vh;
    font-size: 40px;
    left: 80%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }
  .breaker2 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 53vh;
    font-size: 40px;
    left: 80%;
    white-space: nowrap;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 3.3s;
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

  .breaker3 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 71vh;
    font-size: 20px;
    left: 4%;
    white-space: nowrap;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.3s;
  }
  .Painvin{
    position: absolute;
    top: 25vh;
    left: 38%;
    width : 10vw;
    height: 10vh;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.3s;
  }

  </style>