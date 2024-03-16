<script>
  export let index;
</script>

<div class="p12">
    <div class="darker" ></div>
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
        <div class="arrow">
            <img src="hiclipart.com.png" alt="arrow">
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

  .darker {
    background: black;
    opacity:0.1;
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 1;
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
    top: 4vh;
    left: 34%;
    opacity:0;
    animation: fadeInUp 0.3s ease-out forwards;
    animation-delay: 0.5s;
  }
  .intro {
    font-size: 3.417vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roamn;
    color: black;
    text-align: left;
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
      transform: translateX(-2.278vh);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .cipher {
    font-size: 4.556vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    top: 38vh;
    left: 22%;
    opacity:0;
    animation: fadeInLeft 0.5s ease-out forwards;
    animation-delay: 2.3s;
  }
  
  .code {
    font-size: 3.417vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left;
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
      transform: translateX(2.278vh);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .plaintext {
    font-size: 4.556vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    top: 38vh;
    left: 65%;
    opacity: 0;
    animation: fadeInRight 0.5s ease-out forwards;
    animation-delay: 4.3s;
  }
  .decode {
    font-size: 3.417vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: roman;
    color: black;
    text-align: left;
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
    font-size: 3.986vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; 
    font-weight: bold;
    color: black;
    text-align: left;
    max-width: 800px; 
    position: absolute;
    white-space: nowrap;
    top: 85vh;
    left: 12%;
    opacity:0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 7s;
  }

  @keyframes fadeInDown {
    from {
      opacity: 0;
      transform: translateY(-2.278vh);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .arrow{
    position: absolute;
    top: 75vh;
    left: 45vw;
    width : 10vw;
    height: 10vh;
    opacity:0;
    animation: fadeInDown 0.3s ease-out forwards;
    animation-delay: 6.3s;
  }


</style>
