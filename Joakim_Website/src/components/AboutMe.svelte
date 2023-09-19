<script>
    import LoaderAnimation from './LoaderAnimation.svelte';
    import ArrowAnimation from './ArrowAnimation.svelte';

</script>

<div class="Header">
    <h1>About Me</h1>
</div>

<div class="ImageTextHolder">
    <div class="AboutMe">
        <p> Hey, my name is Joakim. 
        I'm a 22 year old student at Halmstad University, currently pursuing my master's in
        Artificial Intelligence and Software Engineering. I'm a very curious person and I love
        to learn new things, especially when it comes to programming and software development.
        </p>

        <div class="MyProgrammingLanguages">
            <div class="RowContainer">
                <h2>></h2>
                <p class="RowItem">Knowledgeable in Java, Python, C++, C, SQL </p>
            </div>
            <div class="RowContainer">
                <h2>></h2>
                <p class="RowItem">Learning Rust, HTML & CSS</p>
            </div>
        </div>
    </div>

    <img src="me_cropped.jpg" alt="404 me not found :)" class="MeImg"/>

    
</div>

<style>

    .Header {
        text-align: center;
        padding-top: 300px;
        font-family: 'Roboto Mono', monospace;
        color: white;
    }

    .Header h1 {
        border-bottom: 1px solid white;
        display: inline-block;
        width: 56vw;
        padding-bottom: 10px;
    }

    .ImageTextHolder {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto;
        padding-top: 40px;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
    }

    .AboutMe {
        width: 30vw;
        padding-left: 24vw;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
    }

    .MeImg {
        width: 15vw;
        border-radius: 50%;
        padding-left: 5vw;
        height: auto;
        color: #FFF;
    }

    .MyProgrammingLanguages {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto;
        padding-top: 3vw;
        width: 30vw;
        height: 10vw;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
    }

    .RowContainer {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .RowItem {
        padding-right: 1vw; /* Add right margin to create space between elements */
        padding-left: 1vw;

    }

</style>

