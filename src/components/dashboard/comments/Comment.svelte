<script>
  export let date = '';
  export let tytul = '';

</script>

<li
  class="border border-gray-200 bg-white shadow-sm transition p-4  rounded-lg transfrom hover:scale-110 hover:shadow-xl block
text-center xl:text-left xl:flex xl:justify-start"
>
  <div class="flex-none w-full xl:w-20 text-center xl:textl-left">
    <img
      src={`https://i.pravatar.cc/100?img=` + Math.floor(Math.random() * 15)}
      alt="Awatar"
      class="rounded-full mb-4 xl:mb-0 inline xl:block"
    />
  </div>
  <div class="flex-grow px-4">
    {#if tytul !== ''}
      <h6 class="font-semibold mb-2">
        {tytul}
      </h6>
    {/if}
    <p class="text-sm">
      <slot />
    </p>
    <div class="text-xs text-gray-500 italic mt-2">
        {#if date !== ''}
            Dodano: {date}
        {/if}
    </div>
  </div>
</li>
