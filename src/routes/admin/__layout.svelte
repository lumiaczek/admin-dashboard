<script>
    import Footer from "../../components/dashboard/nav/Footer.svelte";
    import Menu from "../../components/dashboard/nav/Menu.svelte";
    import PrimaryNav from "../../components/dashboard/nav/PrimaryNav.svelte";
    import SecNav from "../../components/dashboard/nav/SecNav.svelte";
</script>

<div class="flex flex-col h-screen">
    <div class="md:flex">
        <PrimaryNav/>
        <SecNav/>
    </div>
    <div class="flex flex-grow overscroll-y-auto">
        <div class="hidden md:flex items-start justify-between px-8 py-8 bg-blue-800 text-blue-100 md:flex-shrink-0 md:w-56 md:justify-start">
            <div class="relative">
                <Menu/>
                <Footer/>
            </div>
        </div>
        <div class="w-full p-0 bg-gray-100 py-0 md:py-8 overscroll-y-auto">
            <div class="p-4 md:py-0 md:px-12">
                <section>
                    <slot></slot>
                </section>
            </div>
        </div>
    </div>
</div>