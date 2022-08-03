<script>
    export let buttonTitle;
    export let title;
    let isVisible = false;

    const handleClick = () => {
        if(!isVisible){
            isVisible = true;
        }
        else{
            isVisible = false;
        }
    }

    const onKey = (e) => {
        if(e.keyCode == 27){
            isVisible = false;
        }
    }

</script>

<button class="btn btn-primary mt-8" on:click={handleClick}>
    {buttonTitle}
</button>

<div class="fixed top-0 left-0 z-40 w-screen h-screen bg-black bg-opacity-60 backdrop-filter backdrop-blur-lg flex justify-center items-center" class:hidden={isVisible === false}>
    <div class="w-full h-full md:h-auto overflow-y-auto md:w-5/6 lg:w-3/4 2xl:w-1/2 rounded shadow-lg p-8 bg-white text-black">
        <h3 class="inline-flex w-full font-bold text-xl justify-between items-center border-b mb-3 pb-3">
            <span>
                {title}
            </span>

            <span on:click={handleClick} class="font-bold text-sm text-gray-400 hover:text-gray-900 cursor-pointer">
                X
            </span>
        </h3>
        <slot></slot>
    </div>
</div>

<svelte:window on:keydown|preventDefault={onKey} />