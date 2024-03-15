<script>
    export let index;
</script>


<div class="p13">
  {#if index > 11}
    <div class="title">
        <p> Breaking ADFGVX System </p>
    </div>
    <div class="d1">
        <p> Due to the intensive use of the cipher, many messages were sent and received, providing Painvin with enough data to discern patterns.</p>
    </div>
     <div class="d2">
        <p>He broke down the messages into numerical charts and then analyzed the frequency of the numerical charts to determine the corresponding plaintext letters. Finally, the cipher was substituted.</p>
    </div>
    <div class="d3">
        <p> The whole process took him only 2 to 3 months and each message within 2 days.</p>
    </div>
    <div class="d4">
        <p> Now, let's learn system way to decrypt!</p>
    </div>
  {/if}
</div>


<style>
  .p13 {
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

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .title {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 0vh;
    font-size: 50px;
    left: 56%;
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

  .d1 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 1000px;
    top: 13vh;
    font-size: 38px;
    left: 43%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.4s;
  }

  .d2 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 1000px;
    top: 37vh;
    font-size: 38px;
    left: 43%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }
  .d3 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    top: 65vh;
    font-size: 38px;
    left: 20%;
    white-space: nowrap;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
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

  .d4 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    font-size: 32px;
    top: 83vh;
    left: 54%;
    white-space: nowrap;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 4.3s;
  }

  </style>