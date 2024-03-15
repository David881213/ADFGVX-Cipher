<script>
  export let index;
</script>


<div class="p18">
    {#if index > 16}
      <div class="title">Decrypt Step 5: Identifying text</div>
      <div class="subcipher">Substituted cipher: THISISAFUNEXAMPLEGGG</div>
      <div class="sentence">Meaningful Sentence: THIS IS A FUN EXAMPLE GGG.</div>
      <div class="msentence">Remove Padding: THIS IS A FUN EXAMPLE.</div>
      <div class="plain">Finally, we get the Plaintext: "THIS IS A FUN EXAMPLE"</div>
      <div class="w1">The last step of decryption involves using one's own experience and knowledge to make judgments, transforming the substituted ciphertext into meaningful sentences and removing the letters used for padding at the end.</div>
    {/if}
</div>


<style>  
  .p18 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
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
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 5%;
    left: 31%;
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 0.5s;
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

  .w1 {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 35%;
    left: 9%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 2s;
  }

  .plain {
    font-size: 38px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 75%;
    left: 26%;
    text-align: left;
    opacity: 0;
    animation: fadeInLeft 0.7s ease-out forwards;
    animation-delay: 6s;
    white-space: nowrap;
  }

  @keyframes fadeInDown {
    from {
      opacity: 0;
      transform: translateY(-20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .subcipher {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 30%;
    left: 50%;
    text-align: left;
    opacity: 0;
    animation: fadeInDown 0.7s ease-out forwards;
    animation-delay: 3s;
    white-space: nowrap;
  }

  .sentence {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 45%;
    left: 50%;
    text-align: left;
    opacity: 0;
    animation: fadeInDown 0.7s ease-out forwards;
    animation-delay: 4s;
    white-space: nowrap;
  }

  .msentence {
    font-size: 32px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 60%;
    left: 50%;
    text-align: left;
    opacity: 0;
    animation: fadeInDown 0.7s ease-out forwards;
    animation-delay: 5s;
    white-space: nowrap;
  }
  


</style>
