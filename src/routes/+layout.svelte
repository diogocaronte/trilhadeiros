<script>
    import Navbar from '$components/Navbar/Navbar.svelte';
    import '../app.css';
</script>

<header>
    <Navbar />
</header>
<main class="flex-grow bg-gray-900">
    <div class="h-64 lg:h-80 xl:h-96">
        <img class="w-full h-full object-cover" src="/banner.jpg" alt="banner" />
    </div>
    <div class="relative lg:-mt-8 lg:rounded-md bg-gray-100 mx-auto max-w-5xl min-h-[3rem] px-2 lg:px-8 py-8">
        <slot />
    </div>
</main>
<footer class="flex-grow bg-gray-700 text-center">Made with ❤ by Caronte</footer>

<style lang="postcss">
    :global(body > div) {
        @apply min-h-screen grid grid-rows-[auto_1fr_auto];
    }
</style>
