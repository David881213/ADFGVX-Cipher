<script>
  export let index;
  

</script>

<div class="p20">
  {#if index <= 18}
    <div class="background2" ></div>
  {/if}
  
  {#if index > 18}
    <div class="background" ></div>
    <div class="title">
        <p> Effect of the War </p>
    </div>

    <div class="s0">
        <p> The message reveals the intention of German </p>
    </div>

    <div class="s1">
        <p> Stop the last German attack in 1918 </p>
    </div>

    <div class="s2">
        <p> Lay the foundation for the victory of the Allies in WWI </p>
    </div>

  {/if}
  {#if index > 19}
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
  

  .p20 {
    background: transparent;
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
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    white-space: nowrap;
    top: -3vh;
    left: 38%;
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
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

  .s0 {
    font-size: 3.417vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    top: 12vh;
    left: 32%;
    opacity: 0;
    animation: fadeInRight 1s ease-out forwards;
    animation-delay: 1.2s;
  }

  .s1 {
    font-size: 3.417vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    top: 70vh;
    left: 36%;
    opacity: 0;
    animation: fadeInRight 1s ease-out forwards;
    animation-delay: 13s;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .s2 {
    font-size: 4.556vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    top: 80vh;
    left: 20%;
    opacity: 0;
    animation: fadeIn 1s ease-out forwards;
    animation-delay: 14s;
    white-space: nowrap;
  }

  
</style>