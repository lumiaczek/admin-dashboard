<script>
    import Logo from "../../utils/Logo.svelte";
    import Footer from "./Footer.svelte";
    import Menu from "./Menu.svelte";

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

<svelte:head>
    <script src="https://kit.fontawesome.com/0adb7c2a19.js" crossorigin="anonymous"></script>
</svelte:head>

<nav class="flex items-center justify-between text-blue-200 bg-blue-900 border-b border-blue-700 shadow z-30 p-4 md:flex-shrink-0
md:w-56 md:py-0 md:px-8 md:justify-start">
    <Logo/>

    <div class="flex justify-end relative w-3/4 md:hidden">
        <i class="fa-solid fa-bars text-2xl cursor-pointer select-none" on:click={handleClick}></i>

        <div class="absolute top-8 right-0 z-50 text-center" class:hidden={isVisible === false}>
            <div class="bg-blue-800 p-5 rounded shadow-xl border border-blue-700 font-normal">
                <Menu/>
                <Footer/>
            </div>
        </div>
    </div>
</nav>

<svelte:window on:keydown|preventDefault={onKey} />