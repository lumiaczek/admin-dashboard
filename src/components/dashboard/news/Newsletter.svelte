<script>
    import Input from "../../form/Input.svelte";
    import Button from "../../utils/Button.svelte";

    export let title = '';
    export let subtitle = '';
</script>

<div class="bg-gradient-to-l from-gray-900 to-gray-800 block xl:flex justify-between items-center p-8 shadow rounded-lg">
    <div class="w-full xl:w-1/2">
        <h2 class="font-semibold text-xl xl:text-2xl pr-0 lg:pr-5 text-gray-100 flex justify-start items-center">
            {title}
        </h2>
        <h3 class="pr-0 mt-1 lg:pr-5 text-gray-300 flex justify-start items-center">
           {subtitle}
        </h3>
    </div>
    <div class="w-full xl:w-1/2 mt-5 xl:ml-0 transition .transfrom hover:scale-105 text-right xl:pl-8">
        <Input type={"email"} label={"Podaj swój adres email"} class={"border px-3 py-2 rounded-lg w-full "}/>
        <Button className={"success"} tekst={"Zapisz się"} klasa={"mt-5"}/>
    </div>
</div>