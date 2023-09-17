<script>

</script>

<div class="Expertise">
    <h1 class="AboutMe"> About Me </h1>
    <div class="container">
        <div class="box">
            <div class="box-icon">
                <i class="devicon-arduino-plain"></i>
            </div>
            <div class="box-text">
                <h2>Student</h2>
                <p>Pursuing my master's degree in Artificial Intelligence at Halmstad University.</p>
            </div>
        </div>
        
        <div class="box">
            <div class="box-icon">
                <i class="devicon-arduino-plain"></i>
            </div>
            <div class="box-text">
                <h2>Programming Language</h2>
                <p>
                    Skilled in developing software in C, C++, Python and Java. Currently further sharpening my
                    skills in Python and C++. Also trying to learn more about Svelte. ---- ADD ICONS!!
                </p>
            </div>
        </div>
    

    </div>
</div>

<style>
    .AboutMe {
        display: inline-block;
        font-size: xx-large;
        font: 'Roboto Mono';
    }

    .Expertise {
    position: absolute;
    top: 900px;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    color: white;
    font-family: 'Roboto Mono', monospace;
    }

    .container {
        display: flex;
        flex-wrap: nowrap; /* Prevent wrapping to the next line */
        justify-content: space-between;
    }

    .box {
        border: 3px solid #fff;
        padding: 20px;
        margin-bottom: 20px;
    }

    .box-icon {
        text-align: center;
    }

    .box-text h2 {
        font-size: 18px;
        margin-top: 10px;
    }

    .box-text p {
        font-size: 14px;
        margin-top: 10px;
    }
</style>

