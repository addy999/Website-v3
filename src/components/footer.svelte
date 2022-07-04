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
        <a href="http://linkedin.com/in/addybhatia" target="blank_"><img src="./icons8-linkedin-96.png" alt="linkedin"/></a>
    </div>
</footer>

<style>

    footer {
        padding: 36px;
        background-color: #DA62C4
    }

    div {
        width: 60vw;
        display: flex;
        align-items: center;
        margin: auto;
    }

    button, a {
        background-color: transparent;
        width: 25px;
        margin: auto;
        padding: 0px;
    }

    @media (min-width: 600px) {
        button, a {
            width: 30px;
        }
    }
    

</style>