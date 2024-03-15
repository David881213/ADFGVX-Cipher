<script>
  import mapboxgl from 'mapbox-gl';
  import { onMount } from 'svelte';

  export let index;

  

  onMount(() => {
    mapboxgl.accessToken = "pk.eyJ1IjoiaGNlODM1IiwiYSI6ImNsc2wwcDFxdTA5bXUyaXA2eXo4dHc4ZWoifQ.L8O27yjDowwxlIjSIgrQ9A";

    const compiegneCoords = [2.8264, 49.4179];
    const montdidierCoords = [2.5178, 49.6468];

    const VillersBretonneuxCoords = [2.5167, 49.8667]
    const MontdidierCoords = [2.5178, 49.6468]
    const NoyonCoords = [3.0008, 49.5812]
    const SoissonsCoords = [3.3234, 49.3817]
    const ReimsCoords = [4.0317, 49.2628]
    const MarleCoords = [3.7710, 49.7395]
    const MouyCoords = [2.3197, 49.3191]

    const map = new mapboxgl.Map({
      container: 'map',
      style: 'mapbox://styles/mapbox/light-v10',
      center: [2.8958, 49.5178], // Adjust as needed
      zoom: 9
    });

    map.on('load', () => {
      
    });
  });


</script>



<div id="map" style="width: 100%; height: 100vh;"> </div>


<svg id="svg-container" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">

  {#if index > 4}

    <text class="german" x="80%" y="20%" font-family="Arial" font-size="30" fill="red">German</text>

    <text class="frence" x="10%" y="80%" font-family="Arial" font-size="30" fill="blue">Frence</text>

    <text class="r1" x="50%" y="35%" font-family="Arial" font-size="30" fill="black">According to the receiving location, Remaugies</text>

    <text class="r2" x="55%" y="40%" font-family="Arial" font-size="30" fill="black">French army aware the location of offense</text>

    <text class="r3" x="9%" y="40%" font-family="Arial" font-size="30" fill="black">It was expected to happended</text>

    <text class="r32" x="9%" y="47.5%" font-family="Arial" font-size="30" fill="black">Between Montdidier and Compiegne</text>

    <text class="r4" x="56%" y="53%" font-family="Arial" font-size="30" fill="black"> Thus, subordinated successfully</text>

    <text class="r5" x="56%" y="57%" font-family="Arial" font-size="30" fill="black">and resisted the offense in merely one day</text>

    <circle class="rem" cx="41.3%" cy="36.5%" r="10" fill="red" opacity="0.4" />

    <circle class="mont" cx="37.4%" cy="35%" r="30" fill="blue" opacity="0.4" />

    <circle class="com" cx="48.5%" cy="63%" r="30" fill="blue" opacity="0.4" />

    <line class="subordinated" x1="37.4%" y1="35%" x2="48.5%" y2="63%" stroke="blue" stroke-opacity="0.5" stroke-width="10" stroke-dasharray="400" />

    <line class="sen1" x1="49.8%" y1="34%" x2="41.3%" y2="36.5%" stroke="black" stroke-opacity="1" stroke-width="3" stroke-dasharray="400" />

    <line class="sen31" x1="35%" y1="46%" x2="37.4%" y2="35%" stroke="black" stroke-opacity="1" stroke-width="3" stroke-dasharray="400" />

    <line class="sen32" x1="35.1%" y1="47.8%" x2="48.5%" y2="63%" stroke="black" stroke-opacity="1" stroke-width="3" stroke-dasharray="400" />

    <line class="sen4" x1="54.8%" y1="56.8%" x2="45%" y2="54%" stroke="black" stroke-opacity="1" stroke-width="3" stroke-dasharray="400" />

  {/if}

  <line x1="37.4%" y1="0%" x2="37.4%" y2="35%" stroke="black" stroke-opacity="0.5" stroke-width="2" stroke-dasharray="5,5" />

  <line x1="37.4%" y1="35%" x2="54.2%" y2="43.8%" stroke="black" stroke-opacity="0.5" stroke-width="2" stroke-dasharray="5,5" />

  <line x1="54.2%" y1="43.8%" x2="66.8%" y2="67.6%" stroke="black" stroke-opacity="0.5" stroke-width="2" stroke-dasharray="5,5" />

  <line x1="66.8%" y1="67.6%" x2="93.7%" y2="83%" stroke="black" stroke-opacity="0.5" stroke-width="2" stroke-dasharray="5,5" />

  <line x1="93.7%" y1="83%" x2="100%" y2="90%" stroke="black" stroke-opacity="0.5" stroke-width="2" stroke-dasharray="5,5" />

  
</svg>


<style> 

  @keyframes drawLine {
    from {
      stroke-dashoffset: 100%;
    }
    to {
      stroke-dashoffset: 0%;
    }
  }

  .subordinated {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 12s;
  }

  .sen1 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 5s;
  }

  .sen31 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 9s;
  }

  .sen32 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 9s;
  }

  .sen4 {
    stroke-dasharray: 100%;
    stroke-dashoffset: 100%;
    animation: drawLine 1s linear forwards;
    animation-delay: 12s;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 0.4;
    }
  }

  .rem {
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 5s;
  }

  .com {
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 9s;
  }
  .mont {
    opacity: 0;
    animation: fadeIn 0.3s ease-out forwards;
    animation-delay: 9s;
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

  .german {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 2s;
  }
  .frence {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 3s;
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

  .r1 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 4s;
  }
  .r2 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 6s;
  }
  .r4 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 10s;
  }
  .r5 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 11s;
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

  .r3 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 7s;
  }
  .r32 {
    opacity: 0;
    animation: fadeInUp 1s ease-out forwards;
    animation-delay: 8s;
  }


</style>
