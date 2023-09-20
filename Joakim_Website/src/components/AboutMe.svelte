<script>
    import MåsWingAnimation from './MåsWingAnimation.svelte';
    import SwingAnimation from './SwingAnimation.svelte';

</script>
<section id="SectionAboutMe">
    <div class="Header">
        <h1>About Me</h1>
    </div>
</section>


<div class="ImageTextHolder">
    <div class="AboutMe">
        <p> Hey, my name is Joakim. 
        I'm a 22 year old student at Halmstad University, currently pursuing my master's in
        Artificial Intelligence and Software Engineering. I'm a very curious person and I love
        to learn new things, especially when it comes to programming and software development.
        </p>

        <div class="MyProgrammingLanguages">
            <div class="RowContainer">
                <MåsWingAnimation/>
                <p class="RowItem1">Knowledgeable in Java, Python, C++, C, SQL.</p>
            </div>
            <div class="RowContainer">
                <SwingAnimation/>
                <p class="RowItem2">Learning Rust, HTML & CSS.</p>
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
        font-size: xx-large;
        padding-bottom: 10px;
        
    }

    .ImageTextHolder {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto;
        padding-top: 40px;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
        background-color: #34495e;
    }

    .AboutMe {
        width: 30vw;
        height: 30vw;
        padding-left: 24vw;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
    }

    .MeImg {
        width: 15vw;
        border-radius: 50%;
        padding-left: 8vw;
        height: auto;
        color: #FFF;
    }

    .MyProgrammingLanguages {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto;
        padding-top: 3vw;
        width: 35vw;
        height: 40vw;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
    }

    .RowContainer {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;

    }

    .RowItem1 {
        padding-left: 0.2vw;
    }

    .RowItem2 {
        padding-left: 0.2vw;
    }

    @media screen and (max-width: 1500px) {
        .MyProgrammingLanguages {
        display: flex;
        flex-direction: column;
        padding-top: 3vw;
        width: 40vw;
        height: 40vw;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
        padding-bottom: 150vw;
    }

    .RowContainer {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
    }

    .RowItem1 {
        padding-left: 1vw;
        
    }

    .RowItem2 {
        padding-left: 2vw;
        
    }

    }

</style>

