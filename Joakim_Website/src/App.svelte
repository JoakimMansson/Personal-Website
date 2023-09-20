<!--
	COLORS
	#0C0032
	#190061
	#240090
	#3500D3
	#282828
 -->

<script>
    import MouseCursor from './components/MouseCursor.svelte';
	import ScrollDownAnimation from './components/ScrollDownAnimation.svelte';

    import Navbar from "./components/Navbar.svelte";
	import AboutMe from './components/AboutMe.svelte';
	import Projects from './components/Projects.svelte';
	import Experience from './components/Experience.svelte';
	import Contact from './components/Contact.svelte';
	
</script>

<main>
	<div class="body">
		<span class="animated-background"></span>
    	<MouseCursor />
    	<Navbar />
    	<div class="Introduction">
			<h1 class="Name">Joakim Månsson</h1>
			<h2 class="Titles">Software Student</h2>
		</div>
		<div class="scroll-icon">
			<ScrollDownAnimation/>
		</div>
		<AboutMe/>
		<div class="scroll-icon">
			<ScrollDownAnimation/>
		</div>
		
		<Experience/>
		<Contact/>
	</div>
    
</main>

<style>



	.Introduction { 
		padding-top: 300px;
		text-align: center;
		color: white;
		font-family: 'Roboto Mono', monospace;
		animation: myNameBounceIn 2s ease 0s 1 normal forwards;
	}

	.Name {
		font-size: 5em;
	}

	.Titles { 
		font-size: 1.5em;
	}

	.scroll-icon {
		display: flex;
		justify-content: center;
		align-items: center;
		padding-top: 150px;
	}

    .animated-background {
        width: 100%;
        height: 100%;
        background-color: rgba(28, 40, 51 ,100);
        position: fixed;
        z-index: -1; /* Set a lower z-index to push it below other content */
    }



	@keyframes myNameBounceIn {
	0% {
		animation-timing-function: ease-in;
		opacity: 0;
		transform: translateY(-250px);
	}

	38% {
		animation-timing-function: ease-out;
		opacity: 1;
		transform: translateY(0);
	}

	55% {
		animation-timing-function: ease-in;
		transform: translateY(-65px);
	}

	72% {
		animation-timing-function: ease-out;
		transform: translateY(0);
	}

	81% {
		animation-timing-function: ease-in;
		transform: translateY(-28px);
	}

	90% {
		animation-timing-function: ease-out;
		transform: translateY(0);
	}

	95% {
		animation-timing-function: ease-in;
		transform: translateY(-8px);
	}

	100% {
		animation-timing-function: ease-out;
		transform: translateY(0);
	}
}

</style>