<script>
    import Card from "./Card.svelte";

    export let views = 0;
    export let words = 0;
    export let chars = 0;
    export let sharing = 0;
</script>

<Card>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-3 article-statistics">
        <Card class={"article-statistics-box"} title={"Wyświetlenia"}>
            <h3>
                <i class="fa-solid fa-eye text-2xl mr-2"></i>
                {views}
            </h3>
        </Card>
        <Card class={"article-statistics-box"} title={"Słowa"}>
            <h3>
                <i class="fa-solid fa-book-open text-2xl mr-2"></i>
                {words}
            </h3>
        </Card>
        <Card class={"article-statistics-box"} title={"Znaki"}>
            <h3>
                <i class="fa-solid fa-magnifying-glass text-2xl mr-2"></i>
                {chars}
            </h3>
        </Card>
        <Card class={"article-statistics-box"} title={"Udostępnienia"}>
            <h3>
                <i class="fa-solid fa-share-nodes text-2xl mr-2"></i>
                {sharing}
            </h3>
        </Card>
    </div>
</Card>