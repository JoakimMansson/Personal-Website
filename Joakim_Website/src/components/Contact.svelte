<script>
    import LetsConnectAnimation from "./LetsConnectAnimation.svelte";
</script>

<section id="SectionContact">
    <div class="Header">
        <h1>
            Contact
        </h1>
    </div>
</section>


<div class="ContainerSocialMedias">
    <div class="ContainerLetsConnect">

        <div>
            <LetsConnectAnimation/>
        </div>
        <div class="Containerh2">
            <h2>
                Connect with me on my socials!
            </h2>
        </div>
    </div>

    <div class="ContainerLetsConnect">
        
        <h2>@JoakimMansson</h2>
        <div>
            <h4>
            
                <a href="https://www.linkedin.com/in/joakim-mansson/" >
                    LinkedIn 
                    <i style="font-size:24px" class="fa">&#xf08c;</i>
                </a>
             
            
        </h4>
        <h4>
            <a href="https://github.com/JoakimMansson">
                GitHub <i style="font-size:24px" class="fa">&#xf09b;</i> 
            </a>
        </h4>
        </div>
        
        
    </div>
    
</div>


<style>




    .Header {
        text-align: center;
        color: white;
        padding-top: 300px;
        font-family: 'Roboto Mono', monospace;
    }

    .Header h1 {
        border-bottom: 1px solid white;
        display: inline-block;
        width: 35vw;
        padding-bottom: 10px;
        font-size: xx-large;
    }


    .ContainerSocialMedias {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
        padding-top: 6vw;
        
    }

    .ContainerLetsConnect {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    @media screen and (max-width: 1000px) {
        .ContainerSocialMedias {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: center;
        font-family: 'Roboto Mono', monospace;
        color: #FFF;
        padding-top: 6vw;
        }

        .ContainerLetsConnect {
        display: flex;
        flex-direction: column;
        align-items: center;
        }
    }



</style>