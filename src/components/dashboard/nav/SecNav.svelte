<script>
    import SearchBar from "./SearchBar.svelte";
    import UserMenu from "./UserMenu.svelte";
</script>

<nav class="flex items-center justify-between p-4 w-full text-sm bg-white border-b border-gray-200 shadow-sm z-30 md:px-12">
    <div class="mr-4 w-1/2 lg:w-1/3">
        <SearchBar/>
    </div>
    <div class="relative">
        <div class="flex items-center cursor-pointer select-none">
            <div class="mr-1 text-gray-800 whitespace-nowrap flex items-center">
                <span class="font-bold">
                    <UserMenu/>
                </span>
            </div>
        </div>
    </div>
</nav>