<script lang="ts">
    import { SvelteToast, toast } from '@zerodevx/svelte-toast'
    import { onMount } from 'svelte';

    onMount(() => {
        const app = new SvelteToast({
            target: document.body
        })
    })
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
        padding: 10px;
        
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
        width: clamp(30px, 5vw, 40px);
        margin: auto;
        padding: 0px;
    }
    

</style>