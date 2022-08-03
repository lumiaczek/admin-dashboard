<script>
    export let label;
    export let placeholder;
</script>
<label for="">
    {#if label !== ''}
    <span class="text-gray-500 text-sm mb-1 block">
        {label}
    </span>
    {/if}
    <textarea name="textarea" placeholder={placeholder} class="border px-3 py-2 rounded-lg w-full"/>
</label>