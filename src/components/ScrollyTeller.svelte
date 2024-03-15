<script>
  // import Scroller from "@sveltejs/svelte-scroller";
  import Map from "./Mapping.svelte";
  import Topic from "./Topic.svelte";
  import P2 from "./P2.svelte";
  import P3 from "./P3.svelte";
  import P4 from "./P4.svelte";
  import P5 from "./P5.svelte";
  import P6 from "./P6.svelte";
  import P7 from "./P7.svelte";
  import P8 from "./P8.svelte";
  import P9 from "./P9.svelte";
  import P10 from "./P10.svelte";
  import P11 from "./P11.svelte";
  import P12 from "./P12.svelte";
  import P13 from "./P13.svelte";
  import P14 from "./P14.svelte";
  import P15 from "./P15.svelte";
  import P16 from "./P16.svelte";
  import P17 from "./P17.svelte";
  

  let count, index, offset, progress;

  let width, height;
  
</script>

<Scroller
  top={0.0}
  bottom={1}
  threshold={0.5}
  bind:count
  bind:index
  bind:offset
  bind:progress
>
  <div class="background" 
       slot="background">
    
    <Map {index} />
    
    <div class="progress-bars">
      <p>current section: <strong>{index + 1}/{count}</strong></p>
      <progress value={count ? (index + 1) / count : 0} />

      <p>offset in current section</p>
      <progress value={offset || 0} />

      <p>total progress</p>
      <progress value={progress || 0} />
    </div>


    

  </div>

  <div class="foreground" slot="foreground">
    
    <section>
      <div> 
        <div><Topic/></div>
      </div>
    </section>
    <section>
      <div> 
        <div><P2 {index} /></div>
      </div>
    </section>
    <section>
      <div><P3 {index} /></div>
    </section>
    <section>
      <div><P4 {index} /></div>
    </section>
    <section>
      <div><P5 {index} /></div>
    </section>
    <section>
      <div><P6 {index} /></div>
    </section>
    <section>
      <div><P7 {index} /></div>
    </section>
    <section>
      <div><P8 {index} /></div>
    </section>
    <section>
      <div><P9 {index} /></div>
    </section>
    <section>
      <div><P10 {index} /></div>
    </section>
    <section>
      <div><P11 {index} /></div>
    </section>
    <section>
      <div><P12 {index} /></div>
    </section>
    <section>
      <div><P13 {index} /></div>
    </section>
    <section>
      <div><P14 {index} /></div>
    </section>
    <section>
      <div><P15 {index} /></div>
    </section>
    <section>
      <div><P16 {index} /></div>
    </section>
    <section>
      <div><P17 {index} /></div>
    </section>
    <section>This is the 18 section.</section>
  </div>
</Scroller>

<style>
  :global(body) {
    margin: 0;
  }

  .background {
    width: 100%;
    height: 100vh;
    position: relative;
    outline: green solid 3px;
  }

  .foreground {
    width: 100%;
    margin: 0 auto;
    height: auto;
    position: relative;
    outline: red solid 3px;
  }

  .progress-bars {
    position: absolute;
    background: rgba(170, 51, 120, 0.2) /*  40% opaque */;
    visibility: visible;
  }

  section {
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.2); /* 20% opaque */
    /* color: white; */
    text-align: center;
    color: black;
    margin: 0 0 0 0;
  }
</style>
