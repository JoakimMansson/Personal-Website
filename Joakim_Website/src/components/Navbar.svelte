<script>
  import BoopActionAnimation from "./BoopActionAnimation.svelte";
</script>
  

<div class="MyButtons">
  <h1 class="MyName" style="display: inline-block;"> >_ JoakimMansson </h1>
  <button class="AboutMe"> About me<sup>1</sup> </button>
  <button class="Experience"> Experience<sup>2</sup> </button>
  <button class="Projects"> Projects<sup>3</sup> </button>
  <button class="Contact"> Contact<sup>4</sup> </button>
</div>

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
    padding: 1vw 1vw; /* Adjust padding for buttons */
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .MyButtons button:not(:last-child) {
    margin-right: 3vw; /* Add space between buttons (except the last one) */
  }
  
  
  /* Add margin to push the buttons further to the right */
  .MyButtons .MyName + button {
    margin-left: 18%;
  }


  .AboutMe:hover {
    animation: myAnim 2s ease 0s 1 normal forwards;
  }

  .Experience:hover {
    animation: myAnim 2s ease 0s 1 normal forwards;
  }

  .Projects:hover {
    animation: myAnim 2s ease 0s 1 normal forwards;
  }

  .Contact:hover {
    animation: myAnim 2s ease 0s 1 normal forwards;
  }

  @keyframes myAnim {
	0%,
	100% {
		transform: translateY(0);
	}

	10%,
	30%,
	50%,
	70% {
		transform: translateY(-10px);
	}

	20%,
	40%,
	60% {
		transform: translateX(10px);
	}

	80% {
		transform: translateY(8px);
	}

	90% {
		transform: translateX(-8px);
	}
}

</style>
  
 
