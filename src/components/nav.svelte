<script lang="ts">
    import { SvelteToast, toast } from '@zerodevx/svelte-toast';
    import { onMount } from 'svelte';

    onMount(() => {
        const app = new SvelteToast({
            target: document.body
        })
    });

    const onShowcase = () => {
        toast.push(
            "Coming soon!", {
                classes: ['toast']
            }
        )
    }

</script>   

<nav>
    <ul>
        <li><a href="#showcase" on:click={onShowcase}>Showcase</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<style>

    nav {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        padding: 10px;
        padding-right: 20px;
        color: white;
    }

    ul {
        display: flex;
        gap: 5rem;
        justify-content: right;
        list-style-type:none
    }

    li, a {
        color: white;
    }

</style>