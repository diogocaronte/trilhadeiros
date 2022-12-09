<script>
    let links = [
        { link: '', name: 'Gestão de Riscos e Prevenção de Acidentes no Montanhismo' },
        { link: '', name: 'Curso Básico de Montanhismo - CBM' },
        { link: '', name: 'Identificação e Rastros de Animais' },
        { link: '', name: 'Planejamento e Organização de Saídas de Instrução' },
        { link: '', name: 'Alimentação e Cozinha Outdoor' },
        { link: '', name: 'Fotografia Outdoor Básica ' },
        { link: '', name: 'Primeiros Socorros em Áreas Remotas' },
        { link: '', name: 'Planejamento, Navegação e Orientação Terrestre' },
        { link: '', name: 'Nós, Voltas, Amarrações e Ancoragens para Transposições no Trekking' },
        { link: '', name: 'Equipamentos e Técnicas Básicas de Excursionismo' },
        { link: '', name: 'Ética e Mínimo Impacto' },
        { link: '', name: 'Radiocomunicação na Montanha' },
        { link: '', name: 'Meteorologia de Montanha' },
        { link: '', name: 'Navegação em Trilhas com GPS' },
        { link: '', name: 'Programa de Oficinas Básicas Teóricas de Trekking - OBTT' },
        { link: '', name: 'Prevenção e Cuidados com Animais Peçonhentos' },
    ];
</script>

<body>
    <table class="table-auto pt-2 hover:text-black-600 border-collapse flex-initial min-w-full">
        <thead class="underline text-blue-600 decoration-solid">
            <tr>
                <th />
            </tr>
        </thead>
        <tbody class="">
            {#each links as link}
                <tr class="">
                    <td class="p-1 border border-slate-300">
                        <a href="/" class="underline text-blue-600 decoration-solid">{link.name}</a>
                    </td>
                </tr>
            {/each}
        </tbody>
    </table>
</body>
