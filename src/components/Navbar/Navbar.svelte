<script>
    import Hamburguer from './Hamburguer.svelte';

    export let isMobileOpen = false;

    export let links = [
        {
            text: 'Pré Interesse',
            href: '#',
        },
        {
            text: 'Inicial',
            href: '#',
        },
        {
            text: 'Quem Somos',
            href: '/quem-somos',
        },
        {
            text: 'Agenda',
            href: '/agenda',
        },
        {
            text: 'Relatos',
            href: '/relatos',
        },
        {
            text: 'Artigos',
            href: '/artigos',
        },
        {
            text: 'Cursos',
            href: '/cursos',
        },
        {
            text: 'Contato',
            href: '/contato',
        },
        {
            text: 'Faça Parte',
            href: '/faca-parte',
        },
    ];
</script>

<nav class="bg-gray-700">
    <div class="mx-auto max-w-7xl px-2 lg:px-8">
        <div class="relative flex h-16 items-center">
            <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
                <Hamburguer bind:open={isMobileOpen} />
            </div>
            <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
                <div class="hidden sm:ml-6 sm:block">
                    <div class="flex space-x-4">
                        <!-- <a
                            href="#"
                            class="bg-gray-900 text-white px-3 py-2 rounded-md text-sm font-medium"
                            aria-current="page">Dashboard</a
                        > -->

                        {#each links as link}
                            <a
                                href={link.href}
                                class="text-gray-300 hover:bg-gray-600 hover:text-white px-3 py-2 rounded-md text-sm font-medium"
                                >{link.text}</a
                            >
                        {/each}
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Mobile menu, show/hide based on menu state. -->
    <div class="sm:hidden" class:hidden={!isMobileOpen} id="mobile-menu">
        <div class="space-y-1 px-2 pt-2 pb-3">
            <!-- <a
                href="#"
                class="bg-gray-900 text-white block px-3 py-2 rounded-md text-base font-medium"
                aria-current="page">Dashboard</a
            > -->
            {#each links as link}
                <a
                    href={link.href}
                    class="text-gray-300 hover:bg-gray-600 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
                    >{link.text}</a
                >
            {/each}
        </div>
    </div>
</nav>
