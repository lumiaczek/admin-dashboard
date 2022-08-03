<script>
    import PaginationItem from "./PaginationItem.svelte";
</script>

<div class="inline-block">
    <ul class="flex justify-start">
        <PaginationItem>
            <i class="fa-solid fa-angle-left"></i>
        </PaginationItem>

        <PaginationItem class={"hidden"}>1</PaginationItem>
        <PaginationItem>2</PaginationItem>

        <PaginationItem>...</PaginationItem>

        <PaginationItem>25</PaginationItem>
        <PaginationItem>26</PaginationItem>

        <PaginationItem>
            <i class="fa-solid fa-angle-right"></i>
        </PaginationItem>


    </ul>
</div>