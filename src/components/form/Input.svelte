<script>
    export let label = '';
    export let type;
    let clazz;
    export {clazz as class}
    export let placeholder = "";
    if(type == ""){
        type == "text";
    }
</script>
<label for="">
    {#if label !== ''}
    <span class={"text-gray-500 text-sm mb-1 block "}>
        {label}
    </span>
    {/if}
    <input type="{type}" placeholder={placeholder} class={`${clazz || ''}`}/>
</label>