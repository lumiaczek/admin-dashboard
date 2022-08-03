<script>
    export let label;
    export let options = [];
</script>

<label for="">
    <span class="text-gray-500 text-sm block mb-1">
        {label}
    </span>
    <select name="select" id="select" class="border px-3 py-2 rounded-lg w-full">
        {#each options as {value, option}}
        <option value="{value}">
            {option}
        </option>
        {/each}
    </select>
</label>