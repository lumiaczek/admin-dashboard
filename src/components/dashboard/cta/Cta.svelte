<script>
    import Card from "../../utils/Card.svelte";

    export let title = '';
    export let subtitle = '';
    export let call;
    export let url;

</script>

<svelte:head>
    <script src="https://kit.fontawesome.com/0adb7c2a19.js" crossorigin="anonymous"></script>
</svelte:head>

<div class="bg-gradient-to-r from-blue-100 to-blue-200 block shadow rounded-lg mb-4 ">
    <div class="group block xl:flex justify-between items-center p-8">
        <div class="mw-1/2">
            <h2 class="font-semibold text-xl xl:text-2xl pr-0 lg:pr-5 text-blue-900 flex justify-start items-center">
                {title}
            </h2>
            <h3 class="font-bold pr-0 lg:pr-5 text-blue-500 flex justify-start items-center">
                {subtitle}
            </h3>
        </div>
        <div class="mt-5 xl:mt-0 transition group-hover:transform group-hover:rotate-6">
            <a href="{url}" class="btn btn-primary self-stretch">
                <i class="fa-solid fa-circle-check text-md"></i>
                <span class="ml-3">{call}</span>
            </a>
        </div>
    </div>
</div>

<Card>
    <div class="text-center">
        <div class="text-center pt-3 flex justify-center">
            <div class="w-10">
                <i class="fa-solid fa-gear text-3xl text-blue-600 animate-spin mr-3"></i>
            </div>
        </div>

        <div class="mt-5">
            <strong>
                Trwa pobieranie danych z serwera
            </strong>
        </div>
        <p class="text-gray-500">
            Proszę czekać...
        </p>
    </div>
</Card>