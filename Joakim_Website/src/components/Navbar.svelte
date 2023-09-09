<script>

</script>
  
  <style>
    /* CSS styles go here */
    .MyName {
      display: inline-block;
      margin-left: 1%;
      font-size: xx-large;
      color: #fff;
    }
  
    .MyButtons {
      display: flex; /* Use flexbox for horizontal alignment */
      align-items: center; /* Vertically align items in the middle */
    }
  
    .MyButtons button {
      padding: 10px 20px; /* Adjust padding for buttons */
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  
    .MyButtons button:not(:last-child) {
      margin-right: 40px; /* Add space between buttons (except the last one) */
    }
  
  
    /* Add margin to push the buttons further to the right */
    .MyButtons .MyName + button {
      margin-left: 18%;
    }
  </style>
  
  <div class="MyButtons">
    <h1 class="MyName" style="display: inline-block;"> >_ JoakimMansson </h1>
    <button class="AboutMe"> About me<sup>1</sup> </button>
    <button class="Experience"> Experience<sup>2</sup> </button>
    <button class="Projects"> Projects<sup>3</sup> </button>
    <button class="Contact"> Contact<sup>4</sup> </button>
  </div>
