<script>
  export let index;
</script>

<div class="page-container">
  <div class="background" ></div>
  
  {#if index > 11}

    
    <div class="content">
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
            <p> The whole decipher process took him about 3 months.</p>
        </div>
        <div class="d4">
            <p> Now, let's learn system way to decrypt!</p>
        </div>
    </div>
  {/if}

  {#if index > 12}
    <div class="background3" ></div>
  {/if}
</div>

<style>
  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }

  .background3 {
    background: black;
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 2;
    opacity:0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 0.3s;
  }


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
    opacity:0.1;
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


  .content {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 2;
    background: transparent;
    width: 100%;
    height: 100%;
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

  .d1 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 1000px;
    top: 13vh;
    font-size: 4.328vh;
    left: 20%;
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
    font-size: 4.328vh;
    left: 20%;
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
    font-size: 4.328vh;
    left: 0%;
    white-space: nowrap;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
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

  .d4 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: 	black;
    position: absolute; 
    width: 100%;
    font-size: 5.695vh;
    top: 79vh;
    left: 0%;
    white-space: nowrap;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 4.3s;
  }

  

  </style>