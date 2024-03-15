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
            <p> Founded by Colonel Fritz Nebel – German radio officer </p>
        </div>
        <div class="s2">
            <p> Used in WWI East Front since March, 1918 </p>
        </div>
    </div>
  {/if}
</div>

<style>

  @keyframes fadeOut {
    from { opacity: 1; }
    to { opacity: 0.2; }
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

  .title, .founder, .s2 {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    color: 	black;
    text-align: center;
    position: absolute;
    left: 5%;
    width: 90%; /* Ensures text is centered */
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
    font-weight: bold;
    top: 10vh;
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
    font-weight: roman;
    top: 35vh;
    font-size: 50px;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .s2 {
    font-weight: roman;
    top: 60vh;
    font-size: 50px;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 2.5s;
  }

  </style>