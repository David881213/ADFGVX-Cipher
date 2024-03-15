<script>
  export let index;
</script>

<div class="page-container">

  {#if index <= 1}
    <div class="background2" ></div>
  {/if}
  {#if index > 1}

    <div class="background" ></div>
    <div class="content">
        <div class="title">
            <p> The Origin of ADFGVX System </p>
        </div>
        <div class="founder">
            <p> The ADFGVX Cipher system is Founded by Colonel Fritz Nebel – German radio officer, it had been used in WWI East Front since March, 1918. </p>
        </div>
        <div class="s2">
            <p> Now, let's learn how to encrypt!</p>
        </div>
        <div class="image">
          <img src="radio_4.jpg" alt="radio officer">
        </div>
    </div>
  {/if}
</div>

<style>
  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }
  .image {
    opacity:0;
    position:absolute;
    top: 25vh;
    left: 51%;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 2.5s;
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
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .title {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: 	black;
    text-align: center;
    position: absolute;
    left: 5%;
    width: 90%;
    font-weight: bold;
    top: 3vh;
    font-size: 50px;
    opacity:0;
    animation: fadeInUp 0.3s ease-out forwards;
    animation-delay: 0.8s;
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

  .founder {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: 	black;
    text-align: left;
    position: absolute;
    width: 600px;
    font-weight: roman;
    top: 25vh;
    left: 11%;
    font-size: 38px;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .s2 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: 	black;
    position: absolute;
    font-weight: roman;
    top: 75vh;
    left: 30%;
    font-size: 50px;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 3.5s;
  }

  </style>