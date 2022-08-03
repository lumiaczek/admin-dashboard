<script>
    let clazz;
    export {clazz as class}
</script>

<li>
    <!-- svelte-ignore a11y-invalid-attribute -->
    <a href="#" class={`btn h-8 mr-1 shadow-sm hover:shadow-lg focus:shadow-lg ${clazz || ''}`}>
        <slot></slot>
    </a>
</li>