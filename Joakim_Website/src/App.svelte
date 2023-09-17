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
    import Navbar from "./components/Navbar.svelte";
	import ExpertiseBoard from './components/ExpertiseBoard.svelte';
	import ProjectsBar from './components/ProjectsBar.svelte';
</script>

<main>
    <div class="animated-background"></div>
    <MouseCursor />
    <Navbar />
    <div class="Introduction">
		<h1 class="Name">Joakim Månsson</h1>
		<h2 class="Titles">Software Student & Enthusiast</h2>
	</div>
	<ExpertiseBoard/>
	<ProjectsBar/>
</main>

<style>

	.Introduction { 
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		text-align: center;
		color: white;
		font-family: 'Roboto Mono', monospace;
	}

	.Name {
		font-size: 5em;
	}

	.Titles { 
		font-size: 1.5em;
	}

    .animated-background {
        width: 100%;
        height: 100%;
        background-color: #0C0032;
        position: fixed;
        animation: backgroundAnimation 5s infinite alternate;
        z-index: -1; /* Set a lower z-index to push it below other content */
    }

    @keyframes backgroundAnimation {
        0% {
            background-color: #0C0032;
        }
        50% {
            background-color: #282828;
        }
        100% {
            background-color: #0C0032;
        }
    }

</style>