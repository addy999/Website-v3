<script>
    import { fade, slide } from "svelte/transition";
    
    export let secondText = False;
</script>

<li>
    {#if !secondText}
        <slot in:slide={{delay: 350}} out:slide={{duration:200}} name="first">
        </slot>
    {:else}
        <slot in:slide={{delay: 350}} out:slide={{duration:200}} name="second">
        </slot>
    {/if}
</li>
