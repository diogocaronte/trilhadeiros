<script lang="ts">
    import { MenuIcon, XIcon } from '@rgossiaux/svelte-heroicons/solid';
    export let open = false;
    export function toggle() {
        open = !open;
    }
</script>

<button
    type="button"
    class="inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
    aria-controls="mobile-menu"
    aria-expanded="false"
    on:click={toggle}
>
    <span class="sr-only">Open main menu</span>
    {#if open}
        <XIcon class="block h-6 w-6" />
    {:else}
        <MenuIcon class="block h-6 w-6" />
    {/if}
</button>
