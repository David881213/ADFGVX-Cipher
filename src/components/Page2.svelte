<script>
  export let index;
</script>


<div class="p2">
    {#if index > 0}
        <div class="hook1">
            <p> A coded message, </p>
        </div>
        <div class="hook2">
            <p>a dispatch,</p>
        </div>
        <div class="hook3">
            <p>a communication hidden that could alter the course of war.</p>
        </div>
        <div class="hook4">
            <p>This isn't a plotline from a movie;</p>
        </div>
        <div class="hook5">
            <p>this is the real-life story of the ADFGVX cipher.</p>
        </div>
    {/if}
</div>


<style>
  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  .p2 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;      
  }

  .hook1, .hook2, .hook3, .hook4, .hook5 {
    font-size: 4.556vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: #FFFFFF;
    text-align: left; 
    position: absolute;
    opacity: 0;
    animation: fadeInUp 0.6s ease-out forwards;
  }

  .hook1 {
    top: 30vh;
    left: 20vw; 
    animation-delay: 0.5s;
  }
  .hook2 {
    top: 30vh;
    left: 42vw; 
    animation-delay: 1.5s;
  }
  .hook3 {
    top: 35vh;
    left: 20vw; 
    animation-delay: 2.5s;
  }
  .hook4 {
    top: 45vh;
    left: 20vw; 
    animation-delay: 4s;
  }
  .hook5 {
    top: 50vh;
    left: 20vw; 
    animation-delay: 5s;
  }

</style>
