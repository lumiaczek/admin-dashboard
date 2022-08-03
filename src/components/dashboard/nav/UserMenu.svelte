<script>

    let isVisible = false;

    const handleClick = () => {
        if(!isVisible){
            isVisible = true;
        }
        else{
            isVisible = false;
        }
    }
</script>

<div class="relative" on:click={handleClick}>
    <strong>Daniel</strong>
    <p class="hidden md:inline">Borowski</p>
    <div class="absolute top-8 right-0 bg-white p-5 rounded shadow-xl border border-gray-100 font-normal " class:hidden = {isVisible === false}>
        <ul>
            <li class="pb-2">
                <a href="none" class="p-1 text-gray-500 hover:text-black focus:text-black">
                    Ustawienia
                </a>
            </li>
            <div class="w-32 bg-gray-300 my-1 border-b inline-block"></div>

            <li>
                <a href="/auth/Login" class="p-1 font-bold text-gray-500 hover:text-red-600 focus:text-red-600">
                    Wyloguj się
                </a>
            </li>
        </ul>
    </div>
</div>