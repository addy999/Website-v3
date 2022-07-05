<script lang="ts">
    import { toast } from '@zerodevx/svelte-toast';

    const onEmail = () => {
        navigator.clipboard.writeText('addy.bhatia@hey.com');
        toast.push(
            "Email copied to clipboard", {
                classes: ['toast']
            }
        )
    }
</script>

<footer id="contact">
    <div>
        <button on:click={onEmail}><img src="./icons8-mail-100.png" alt="email"/></button>
        <a href="http://linkedin.com/in/addybhatia" target="blank_" id="in"><img src="./icons8-linkedin-96.png" alt="linkedin"/></a>
        <a href="https://calendly.com/addybhatia/" target="blank_">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd" />
              </svg>
        </a>
    </div>
</footer>

<style>

    footer {
        padding: 36px;
        background-color: #4F39FA
    }

    img {
        filter: invert(1)
    }

    div {
        width: 60vw;
        display: flex;
        align-items: center;
        margin: auto;
        gap: 2rem
    }

    button, a {
        background-color: transparent;
        width: 25px;
        margin: auto;
        padding: 0px;
        color: white;
    }

    #in {
        width: 27.5px;
    }

    @media (min-width: 600px) {
        button, a {
            width: 30px;
        }

        #in {
            width: 32.5px; 
        }

        div {
            gap: 1.5rem
        }
    }
    

</style>