<script>
    import Card from "../utils/Card.svelte";
    import Pagination from "./Pagination.svelte";
</script>

<div>
    <Card class={"overflow-x-auto mb-5"}>
        <table class="table border-collapse border border-blue-100 w-full bg-white">
            <slot></slot>
        </table>
    </Card>

    <Pagination/>

</div>