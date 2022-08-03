<script>
    export let url = "";
    export let isCurrent = false;
    let clazz;
    export {clazz as class}
</script>

<a href="{url}" class={`truncate bg-white hover:bg-gray-100 focus:bg-gray-100 transition first:rounded-tl first:rounded-bl 
last:rounded-tr last:rounded-bl shadow p-3 flex justify-start ${clazz || ''}`} class:font-semibold={isCurrent==true} >
    <slot></slot>
</a>