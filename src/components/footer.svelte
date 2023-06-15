<script lang="ts">
    import { toast } from '@zerodevx/svelte-toast';
    import { Icon, Mail, Calendar, Camera } from "svelte-hero-icons";

    const onEmail = () => {
        navigator.clipboard.writeText('addy.bhatia@hey.com');
        toast.push(
            "Email copied to clipboard", {
                classes: ['toast']
            }
        )
    }
</script>

<footer>
    <div>
        <button on:click={onEmail}>
            <Icon src="{Mail}" solid />
        </button>
        <a href="http://linkedin.com/in/addybhatia" target="blank_" id="in">
            <img src="./icons8-linkedin-96.png" alt="linkedin"/>
        </a>
        <a href="https://calendly.com/addybhatia/" target="blank_">
            <Icon src="{Calendar}" solid />
        </a>
        <a href="https://instagram.com/addy.and.his.lens/" target="blank_">
            <Icon src="{Camera}" solid />
        </a>
        
    </div>
    <span id="contact" />
</footer>

<style>

    footer {
        padding: 36px;
        background-color: #4F39FA
    }

    img {
        filter: invert(1);
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
    
    @media (min-width: 600px) {
        button, a {
            width: 30px;
        }

        div {
            gap: 1.5rem
        }
    }
    

</style>