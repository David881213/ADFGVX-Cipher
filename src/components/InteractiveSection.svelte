<script>
  import { flip } from 'svelte/animate';
  import { fly } from 'svelte/transition';
  import { cubicOut } from 'svelte/easing';
  import { fade, scale } from 'svelte/transition';
  import { onMount } from 'svelte';
  export let index;
  

  let plaintext = ''; // 用來儲存輸入的明文
  let ciphertext = ''; // 用來儲存加密後的密文

  const tableContent = [
    ['', 'A', 'D', 'F', 'G', 'V', 'X'],
    ['A', 'i', 'w', 'o', 'u', 'l', 'd'],
    ['D', 'e', 'f', 'r', 'y', 'o', 'a'],
    ['F', '9', 'b', 'c', '1', 'g', 'h'],
    ['G', 'j', 'k', '2', 'm', 'n', '7'],
    ['V', 'p', '3', 'q', 's', '6', 't'],
    ['X', '4', 'v', 'x', '5', 'z', '8']
  ];
  
  const size = 7; // 表格的大小
  const gridLength = 250; // 表格的尺寸
  $: showGrid = index > 11;
  $: gridLines = Array.from({ length: size + 1 }); // 创建额外的线条以完成表格

  // 當按下Encrypt按鈕時，調用這個函數來處理加密
  function encrypt() {
    // 這裡可以替換成你的加密邏輯
    ciphertext = plaintext; // 暫時將輸入的明文作為密文顯示
  }

  let startFadeIn = false;

  onMount(() => {
    setTimeout(() => {
      startFadeIn = true;
    }, 3200); // 延遲 3.2 秒後開始淡入
  });

</script>

{#if showGrid}
  <div class="interactive-content" 
          in:fly={{ x: -300, duration: 1000 }}
          out:fly={{ x: -300, duration: 1000}}>
    <div class="plantext_and_buttum" 
          in:fade={{ duration: 1500 }}
          out:fade={{ duration: 1500 }}>
      <h2 style="font-size: 21px">Type in your plaintext:</h2>
      <div class="input-and-button">
        <input type="text" class="plain_input" placeholder="plaintext" bind:value={plaintext}>
        <button class='encrypt_buttun' on:click={encrypt}>Encrypt</button>
      </div>
    </div>
  </div>
{/if}

{#if showGrid}
  <div class="grid-container" style={`grid-template-columns: repeat(${tableContent[0].length}, 1fr);`}>
    {#each tableContent as row, rowIndex}
      {#each row as cell, cellIndex}
        {#if startFadeIn}
          <div in:fade={{ duration: 500 }} class="cell"
               style={`grid-row-start: ${rowIndex + 1}; grid-column-start: ${cellIndex + 1};`}>
            {cell}
          </div>
        {/if}
      {/each}
    {/each}
    {#each gridLines as _, i (i)}
      <div class="horizontal-line" 
           style={`--i: ${i}; top: ${(100 / size) * i}%; 
                  animation-delay: ${(i * 0.1) + 1}s;`}>
      </div>
    {/each}
    {#each gridLines as _, i (i)}
      <div class="vertical-line" 
           style={`--i: ${i}; left: ${(100 / size) * i}%; 
                  animation-delay: ${(i * 0.1) + 1}s;`}>
      </div>
    {/each}
  </div>
{/if}

{#if showGrid}
  <div class="cipher_title"
      in:fly={{ delay: 1700, x: 800, duration: 1500 }}
      out:fly={{ delay: 1700, x: 800, duration: 1500}}>
      <h2 style="font-size: 21px">Your ADFRVX ciphertext: </h2>
      <div class="cipher_text" >
        <p>{ciphertext}</p>
      </div>
  </div>
{/if}

<style>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Koulen&family=Lato&family=Nunito&family=Playfair+Display:ital@1&family=Prata&family=Raleway:ital,wght@1,100&family=Roboto&family=Roboto+Condensed&family=Teko&display=swap');

  .interactive-content {
    padding: 1em;
    border: 1px solid #ccc;
    margin-top: 1em; /* 为交互内容和网格之间留出空间 */
    position: relative;
    font-family: Roboto, sans-serif;
    font-weight: 0;
    font-size: 14px;
  }

  .grid-container {
    display: grid;
    position: relative;
    width: var(--grid-length);  /* Adjust as needed */
    height: var(--grid-length); /* Adjust as needed */
    --grid-length: 300px; /* Or any other size */
    margin: auto;
    margin-top: 10px;
  }

  .cell {
    font-family: Roboto, sans-serif;
    font-size: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: transparent;
    border: 1px solid #ccc;
    opacity: 0; /* 確保初始狀態為不可見 */
    animation: fadeIn 0.5s ease-in-out forwards;
    }

  .horizontal-line {
    position: absolute;
    background: black;
    height: 1px;
    width: 0;
    animation: drawHorizontalLine 0.5s forwards;
  }
  .vertical-line {
    position: absolute;
    background: black;
    width: 1px;
    height: 0;
    animation: drawVerticalLine 0.5s forwards;
  }

  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }
  @keyframes drawHorizontalLine {
    to { width: 100%; }
  }
  @keyframes drawVerticalLine {
    to { height: 100%; }
  }

  .encrypt_buttun {
    font-family: Roboto, sans-serif;
    font-weight: 0;
    font-size: 20px;
    color: #fff;
    background: linear-gradient(90deg, #0066CC 0%, #c500cc 100%);
    padding: 10px 30px;
    border: 2px solid #0066cc;
    box-shadow: rgb(0, 0, 0) 0px 0px 0px 0px;
    border-radius: 50px;
    transition : 1000ms;
    transform: translateY(0);
    display: flex;
    flex-direction: row;
    align-items: center;
    cursor: pointer;
  }

  .encrypt_buttun:hover{
    transition : 1000ms;
    padding: 10px 50px;
    transform : translateY(-0px);
    background: linear-gradient(90deg, #0066CC 0%, #c500cc 100%);
    color: #0066cc;
    border: solid 2px #0066cc;
  }

  .plain_input {
    font-family: Roboto, sans-serif;
    outline:0;
    color: #333333;
    font-size: 20px;
    padding: 10px 70px;
    width: 300px;
    border-radius: 50px;
    border: 0px solid #d6d6d6;
    transition : 1000ms;
    transform: translateY(0);
    background-color: #F5F5F5FF;
    margin-right: 30px;
  }
  .plain_input:active, .plain_input:focus {
    transition : 1000ms;
    padding: 10px 100px;
    transform : translateY(-0px);
    background-color: #ffffff;
    color: #000000;
    border: 0px solid #969696;
    width: 400px;
  }

  .plantext_and_buttum {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .input-and-button {
    display: flex;
    align-items: center;
  }

  .cipher_title {
    font-family: Roboto, sans-serif;
    text-align: left;
    padding: 1em;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .cipher_text {
    font-family: Roboto, sans-serif;
    font-size: 20px;
    text-align: left; /* 添加这个属性 */
  }

</style>