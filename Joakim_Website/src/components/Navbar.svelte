<script>
  function scrollIntoView({ target }) {
		const el = document.querySelector(target.getAttribute('href'));
		if (!el) return;
    el.scrollIntoView({
      behavior: 'smooth'
    });
  }
</script>
  

<div class="NavBar">
  <h1 class="MyName"> >_ JoakimMansson </h1>
  <div class="MyButtons">
    <button href="#SectionAboutMe" class="AboutMe" on:click|preventDefault={scrollIntoView}> About me<sup>1</sup> </button>
    <button href="#SectionExperience" class="Experience" on:click|preventDefault={scrollIntoView}> Experience<sup>2</sup> </button>
    <!--<button href="#SectionProjects" class="Projects" on:click|preventDefault={scrollIntoView}> Projects<sup>3</sup> </button> -->
    <button href="#SectionContact" class="Contact" on:click|preventDefault={scrollIntoView}> Contact<sup>3</sup> </button>
  </div>
</div>


<style>
  
  .NavBar {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center; /* Vertically align items in the middle */
    padding: 20px; /* Add padding as needed */
    background-color: #34495e;
  }

  .MyName {
    display: inline-block;
    margin-left: 1%;
    font-size: xx-large;
    color: #fff;
    margin-right: auto;
  }
  
  .MyButtons {
    display: flex;
    flex-direction: row;
    align-items: center; /* Vertically align items in the middle */
  }
  
  .MyButtons button {
    padding: 1vw 1vw; /* Adjust padding for buttons */
    font-size: 1vw;
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
  
 
