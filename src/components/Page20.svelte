<script>
  export let index;
  

</script>

<div class="p20">
  {#if index > 18}
    <div class="title">
        <p> Effect of the War </p>
    </div>

    <div class="s0">
        <p> The message reveals the intention of German </p>
    </div>

    <div class="s1">
        <p> Stop the last German attack in 1918. </p>
    </div>

  {/if}
</div>

<style>
  

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
    color: black;
    text-align: left; /* Align text to the left */
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
      transform: translateX(20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .s0 {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 12vh;
    left: 32%;
    opacity: 0;
    animation: fadeInRight 1s ease-out forwards;
    animation-delay: 1.2s;
  }

  .s1 {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 70vh;
    left: 36%;
    opacity: 0;
    animation: fadeInRight 1s ease-out forwards;
    animation-delay: 13s;
  }

  
</style>