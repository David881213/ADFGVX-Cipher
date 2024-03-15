<script>
  export let index;
</script>


<div class="p21">
    {#if index > 19}
        <div class="hook1">
            <p> Ending</p>
        </div>
        <div class="hook2">
            <p>The ADFGVX cipher is an early example of the types of encryptions that are foundational to modern cryptographic practices.</p>
        </div>
        <div class="hook3">
            <p>By practicing encrypt and decrypt, we learn the value of both complexity and simplicity in encryption, as overly complex systems can lead to operational failures, while overly simple may be decipher.</p>
        </div>
        <div class="hook4">
            <p>The decryption of ADFGVX cipher underscores the critical role of cryptanalysis and the impact of intelligence gathering in warfare.</p>
        </div>
        <div class="hook5">
            <p>And demonstrates the importance of adapting and evolving cryptographic methods to maintain secrecy.</p>
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
  
  .p21 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;      
  }

  .hook1, .hook2, .hook3, .hook4, .hook5 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: #FFFFFF;
    text-align: left; 
    position: absolute;
    opacity: 0; /* Start elements as invisible */
    animation: fadeInUp 0.6s ease-out forwards; /* Apply the animation */
  }

  .hook1 {
    font-size: 50px;
    font-weight: bold;
    top: 0vh;
    left: 44%; 
    animation-delay: 0.5s; /* Delay the animation */
  }
  .hook2 {
    font-size: 32px;
    font-weight: roman;
    top: 19vh;
    left: 5%; 
    animation-delay: 1.5s; /* Delay the animation */
  }
  .hook3 {
    font-size: 32px;
    font-weight: roman;
    top: 39vh;
    left: 5%; 
    animation-delay: 2.5s; /* Delay the animation */
  }
  .hook4 {
    font-size: 32px;
    font-weight: roman;
    top: 59vh;
    left: 5%; 
    animation-delay: 4s; /* Delay the animation */
  }
  .hook5 {
    font-size: 32px;
    font-weight: roman;
    top: 79vh;
    left: 5%; 
    animation-delay: 5s; /* Delay the animation */
  }

</style>
