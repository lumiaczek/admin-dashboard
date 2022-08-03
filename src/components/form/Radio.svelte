<script>
    export let name;
    export let label;
</script>

<label class="flex justify-start items-center" for="">
    <input class="mr-1" type="radio" name="{name}" id="{name}">
    <span class="text-gray-500 text-sm">
        {label}
    </span>
</label>