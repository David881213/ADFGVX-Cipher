<script>
  export let index;
</script>

<div class="p12">
    {#if index > 10}
        <div class="title">
            <p> Key Decode Information </p>
        </div>
        <div class="cipher">
            <p> Cipher </p>
        </div>
        <div class="plaintext">
            <p> Plaintext </p>
        </div>
        <div class="intro">
            <p> Painvin had decode one most critical message from German cryptogram </p>
        </div>
        <div class="code">
            <p> FGAXA XAXFF FAFVA AVDFA GAXFX FAFAG DXGGX AGXFD XGAGX GAXGX AGXVF VXXAG XDDAX GGAAF DGGAF FXGGX XDFAX GXAXV AGXGG DFAGG GXVAX VFXGV FFGGA XDGAX FDVGG A </p>
        </div>
        <div class="decode">
            <p> Munitionierung beschleunigen Punkt Soweit nicht eingesehen auch bei Tag </p>
        </div>
        <div class="meaning">
            <p> Which mean: Speed up supply of ammunition. If not seen also during the day </p>
        </div>
    {/if}
</div>

<style>
  .p12 {
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
    top: 4vh;
    left: 34%;
    opacity:0;
    animation: fadeInUp 0.3s ease-out forwards;
    animation-delay: 0.5s;
  }
  .intro {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roamn;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    white-space: nowrap;
    top: 25vh;
    left: 26%;
    opacity:0;
    animation: fadeInUp 0.5s ease-out forwards;
    animation-delay: 1.3s;
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

  .cipher {
    font-size: 40px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 38vh;
    left: 22%;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }
  
  .code {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 48vh;
    left: 4%;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 3.3s;
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

  .plaintext {
    font-size: 40px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 38vh;
    left: 65%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 4.3s;
  }
  .decode {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    top: 51vh;
    left: 53%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 5.3s;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .meaning {
    font-size: 30px;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left; /* Align text to the left */
    max-width: 800px; 
    position: absolute;
    white-space: nowrap;
    top: 75vh;
    left: 20%;
    opacity:0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 6.3s;
  }
</style>
