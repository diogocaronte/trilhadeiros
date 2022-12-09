<script>
    export let title = '';
    export let body = '';
    export let link = '';
    export let link_title = '';
</script>

<div class="p-5">
    <div class="underline decoration-solid font-semibold">
        <p>{title}</p>
    </div>
    <div class="flex">
        <p>{body}</p>
        <a href={link} class="pl-1 hover:text-blue-600">{link_title}</a>
    </div>
</div>
