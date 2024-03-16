<script>
  let transpositionKey = "13764285";
  let plaintext = 'Try to encrypt this message';
  let solution = '';
  let feedbackMessage = '';
  let ciphertext = 'XAVXD DGAAF DAGDX GAGGF VGGXG AGDDX XAGVA XVXGG XXXAX GGX'
  export let index;


  // Function to check the solution.
  function checkSolution() {
    // Convert both to lowercase and trim whitespace before comparing
    let formattedSolution = solution.replace(/\s+/g, '').toLowerCase();
    let formattedciphertext = ciphertext.replace(/\s+/g, '').toLowerCase();

    if (formattedSolution === formattedciphertext) {
      feedbackMessage = 'Correct! Congratulations!!';
    } else {
      feedbackMessage = 'Wrong, please try again.';
    }
  }

  // Example function to handle form submission.
  function handleSubmit() {
    checkSolution();
  }

  let showciphertext = false;

  function togglePlaintext() {
    showciphertext = !showciphertext;
  }
</script>

<div class="p10">
  {#if index > 8}
    <div class="form-container open-sans-my-text-style">

    <div class="title">Try to encrypt by yourself!!</div>
    <div class="plain">Plaintext: Try to encrypt this message</div>
    <div class="keyword">Keyword: 13764285</div>

    <div class="label-text">Enter your ciphertext:</div>
    
        <form on:submit|preventDefault={handleSubmit} class="interactive-content">
            <div class="plaintext-and-button">
                <div class="input-and-button">
                <input id="solution-input" type="text" class="plain_input" bind:value={solution} placeholder="Enter ciphertext">
                <button type="submit" class='encrypt_buttun'>Check</button>
                </div>
            </div>

            {#if feedbackMessage}
                <p class="feedback-message">{feedbackMessage}</p>
            {/if}
        </form>
        
        <div class="parent-element">
            
            <button on:click={togglePlaintext} class="toggle-plaintext-button">
                {showciphertext ? 'Hide Solution' : 'Show Solution'}
            </button>

            {#if showciphertext}
                <p class="answer">Ciphertext: {ciphertext}</p>
            {/if}
        </div>
    </div>

    <table class="grid">
            <tr>
                <th></th>
                <th>A</th>
                <th>D</th>
                <th>F</th>
                <th>G</th>
                <th>V</th>
                <th>X</th>
            </tr>
            <tr>
                <th>A</th>
                <td>C</td>
                <td>O</td>
                <td>8</td>
                <td>X</td>
                <td>F</td>
                <td>4</td>
            </tr>
            <tr>
                <th>D</th>
                <td>M</td>
                <td>K</td>
                <td>3</td>
                <td>A</td>
                <td>Z</td>
                <td>9</td>
            </tr>
            <tr>
                <th>F</th>
                <td>N</td>
                <td>W</td>
                <td>L</td>
                <td>0</td>
                <td>J</td>
                <td>D</td>
            </tr>
            <tr>
                <th>G</th>
                <td>5</td>
                <td>S</td>
                <td>I</td>
                <td>Y</td>
                <td>H</td>
                <td>U</td>
            </tr>
            <tr>
                <th>V</th>
                <td>P</td>
                <td>1</td>
                <td>V</td>
                <td>B</td>
                <td>6</td>
                <td>R</td>
            </tr>
            <tr>
                <th>X</th>
                <td>E</td>
                <td>Q</td>
                <td>7</td>
                <td>T</td>
                <td>2</td>
                <td>G</td>
            </tr>
    </table>
  {/if}
    
</div>

<style>
  
  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .p10 {
    background: black;
    height: 100vh; 
    width: 100%;   
    margin: 0;
    position: relative;
  }
  
  .title {
    font-size: 5.695vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: bold;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
    top: 5%;
    left: 31%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 0.5s;
  }

  .plain {
    font-size: 4.328vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 17%;
    left: 5%;
    text-align: left;
    white-space: nowrap;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .keyword {
    font-size: 4.328vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    position: absolute;
    top: 27%;
    left: 5%;
    text-align: left;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .label-text {
    font-size: 4.328vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    max-width: 600px;
    margin: 0;
    text-align: left;
    position: absolute;
    top: 37%;
    left: 5%;
    text-align: left;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  

  
  .form-container {
    flex-grow: 1;
    margin-right: 20px;
  }

  form {
    margin-bottom: 20px;
  }

  .Cipher {
    font-size: 1.5em;
    font-weight: 600;
    font-family: 'IBM Plex Sans', sans-serif; 
    color: white;
    margin-top: 20px;
  }

  .interactive-content {
    position: absolute;
    top: 47%;
    left: 5%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .encrypt_buttun {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: 0;
    font-size: 3.645vh;
    color: #fff;
    background: linear-gradient(90deg, #0066CC 0%, #c500cc 100%);
    padding: 10px 30px;
    border: 2px solid #0066cc;
    box-shadow: rgb(0, 0, 0) 0px 0px 0px 0px;
    border-radius: 50px;
    transition : 1000ms;
    transform: translateY(0);
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
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    outline:0;
    color: #333333;
    font-size: 32px;
    padding: 10px 70px;
    width: 300px;
    border-radius: 50px;
    border: 0px solid #d6d6d6;
    transition : 1000ms;
    transform: translateY(0);
    background-color: #F5F5F5FF;
    margin-right: 30px;
    margin-bottom: 30px;
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

  .feedback-message {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    position: absolute;
  }

  .parent-element {
    position: absolute;
    top: 75%;
    left: 5%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .toggle-plaintext-button {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: 0;
    font-size: 3.645vh;
    color: #fff;
    background: linear-gradient(90deg, #0066CC 0%, #c500cc 100%);
    padding: 10px 30px;
    border: 2px solid #0066cc;
    box-shadow: rgb(0, 0, 0) 0px 0px 0px 0px;
    border-radius: 50px;
    transition : 1000ms;
    transform: translateY(0);
    flex-direction: row;
    align-items: center;
    cursor: pointer;
    margin-bottom: 30px;
  }

  .toggle-plaintext-button:hover{
    transition : 1000ms;
    padding: 10px 50px;
    transform : translateY(-0px);
    background: linear-gradient(90deg, #0066CC 0%, #c500cc 100%);
    color: #0066cc;
    border: solid 2px #0066cc;
  }

  .answer {
    font-size: 3.645vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: roman;
    color: #FFFFFF;
    margin: 0;
    text-align: left;
    position: absolute;
    text-align: left;
    white-space: nowrap;
  }

  .grid {
    border-collapse: collapse;
    color: white;
    position: absolute;
    top: 23%;
    left: 60%;
    opacity: 0;
    animation: fadeIn 0.5s ease-out forwards;
    animation-delay: 1.5s;
  }

  .grid th, .grid td {
    border: 1px solid white;
    width: 6.834vh;  
    height: 6.834vh; 
    text-align: center;
    vertical-align: middle;
  }

  .grid th {
    font-size: 3.189vh;
    font-weight: bold;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  }

  .grid td {
    font-size: 3.189vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-weight: normal;
  }

</style>