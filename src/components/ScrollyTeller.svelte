<script>
  import Scroller from "@sveltejs/svelte-scroller";
  import Map from "./Mapping.svelte";
  import Page1 from "./Page1.svelte";
  import Page2 from "./Page2.svelte";
  import Page3 from "./Page3.svelte";
  import Page4 from "./Page4.svelte";
  import Page5 from "./Page5.svelte";
  import Page6 from "./Page6.svelte";
  import Page7 from "./Page7.svelte";
  import Page8 from "./Page8.svelte";
  import Page9 from "./Page9.svelte";
  import Page10 from "./Page10.svelte";
  import Page11 from "./Page11.svelte";
  import Page12 from "./Page12.svelte";
  import Page13 from "./Page13.svelte";
  import Page14 from "./Page14.svelte";
  import Page15 from "./Page15.svelte";
  import Page16 from "./Page16.svelte";
  import Page17 from "./Page17.svelte";
  import Page18 from "./Page18.svelte";
  import Page19 from "./Page19.svelte";
  import Page20 from "./Page20.svelte";
  import Page21 from "./Page21.svelte";

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
    

  </div>

  <div class="foreground" slot="foreground">
    
    <section>
      <div> 
        <div><Page1/></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page2 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page3 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page4 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page5 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page6 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page7 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page8 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page9 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page10 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page11 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page12 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page13 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page14 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page15 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page16 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page17 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page18 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page19 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page20 {index} /></div>
      </div>
    </section>
    <section>
      <div> 
        <div><Page21 {index} /></div>
      </div>
    </section>
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