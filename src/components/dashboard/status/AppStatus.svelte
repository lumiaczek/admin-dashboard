<script>
    import Card from "../../utils/Card.svelte";

</script>

<svelte:head>
    <script src="https://kit.fontawesome.com/0adb7c2a19.js" crossorigin="anonymous"></script>
</svelte:head>

<Card class={"bg-gradient-to-r from-green-600 to-green-700 p-6"}>
    <h6  class="text-green-100 flex justify-start">
        <i class="fa-solid fa-users mt-0.5"></i>
        <span class="ml-1">
            Nowi użytkownicy
        </span>
    </h6>
    <p class="text-white text-5xl">
        {Math.floor(Math.random() * 15)}
    </p>
</Card>

<Card class={"bg-gradient-to-r from-red-600 to-red-700 p-6"}>
    <h6  class="text-red-100 flex justify-start">
        <i class="fa-solid fa-newspaper mt-1"></i>
        <span class="ml-1">
            Nowe artykuły
        </span>
    </h6>
    <p class="text-white text-5xl">
        {Math.floor(Math.random() * 15)}
    </p>
</Card>

<Card class={"bg-gradient-to-r from-blue-600 to-blue-700 p-6"}>
    <h6  class="text-blue-100 flex justify-start">
        <i class="fa-solid fa-building mt-1"></i>
        <span class="ml-1">
            Nowi klienci
        </span>
    </h6>
    <p class="text-white text-5xl">
        {Math.floor(Math.random() * 15)}
    </p>
</Card>

<Card class={"bg-gradient-to-r from-yellow-600 to-yellow-700 p-6"}>
    <h6  class="text-yellow-100 flex justify-start">
        <i class="fa-solid fa-message mt-1"></i>
        <span class="ml-1">
            Nowe komentarze
        </span>
    </h6>
    <p class="text-white text-5xl">
        {Math.floor(Math.random() * 15)}
    </p>
</Card>