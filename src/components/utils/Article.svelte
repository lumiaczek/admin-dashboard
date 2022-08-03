<script>
    import Card from "./Card.svelte";
    import ArticleFooter from "./ArticleFooter.svelte";
    import AlertSuccess from "./AlertSuccess.svelte";

    export let title = "";
    export let author = "";
    export let date = "";

    let alertSuccessShown = false;
    let alertDangerShown = false;

</script>

<Card class={"article"}>
    <h1 class="article-title">
        {title}
    </h1>

    <section class="article-data">
        <div>
            {author}, {date}
        </div>
        <div class="inline-flex space-x-2 mt-5">
            <button class="btn btn-success" on:click={() => alertDangerShown == true}>
                Udostępnij artykuł
            </button>
            <button class="btn btn-info" on:click={() => alertSuccessShown == true}>
                Zapisz na później
            </button>
        </div>
    </section>

    <article class="article-content">
        <slot></slot>
    </article>

    <footer class="article-footer">
        <ArticleFooter
            views={Math.floor(Math.random() * 100)}
            words={"435"}
            chars={"2150"}
            sharing={Math.floor(Math.random() * 15)}
        />
    </footer>
</Card>

