<!-- App.svelte -->
<script>
    let randomNum = Math.floor(Math.random() * 100) + 1;
    // Generate a random number between 1 and 100
    function generateRandomNum() {
      randomNum = Math.floor(Math.random() * 100) + 1;
    }
    // Function to generate a new random number on button click
  </script>
  
  <div class="center">
    <h1>{randomNum}</h1>
    <button on:click={generateRandomNum}>Generate New Number</button>
  </div>
  
  <style>
    .center {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    h1 {
      font-size: 10rem;
      margin-bottom: 2rem;
    }
    button {
      font-size: 1.5rem;
      padding: 0.5rem 1rem;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>