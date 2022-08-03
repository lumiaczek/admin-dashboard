<script>
    import Article from "../../components/utils/Article.svelte";
    import BreadcrumbsItem from "../../components/utils/BreadcrumbsItem.svelte";

</script>

<div class="bg-blue-100 shadow rounded mb-4 p-4 flex justify-start items-center truncate">
    <BreadcrumbsItem url={"/"}>
        <i class="fa-solid fa-house text-2xl"></i>
    </BreadcrumbsItem>
    <BreadcrumbsItem url={"/admin"} class={"text-gray-500"}>
        <span class="ml-2">
            Panel Administracyjny
        </span>
    </BreadcrumbsItem>
    <BreadcrumbsItem url={"/regulation"} isCurrent={true}>
        <span class="ml-2">
            Regulamin
        </span>
    </BreadcrumbsItem>
</div>

<div class="grid grid-cols-1">
    <Article
        title={"Regulamin naszej usługi"}
        author={"Daniel Borowski"}
        date={"2022-08-31"}
    >
        <p class="article-p">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum tempora error ab? Recusandae distinctio optio omnis alias ea labore voluptatem architecto similique minima velit, numquam maxime eum enim reprehenderit ducimus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis laudantium ipsam numquam, obcaecati optio nam velit veritatis explicabo commodi consequatur nesciunt accusantium itaque voluptatibus saepe quis qui alias! Cum, explicabo!
        </p>

        <p class="article-p">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum tempora error ab? Recusandae distinctio optio omnis alias ea labore voluptatem architecto similique minima velit, numquam maxime eum enim reprehenderit ducimus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae tempore possimus laudantium. Aut cumque ipsam beatae adipisci aspernatur nesciunt, iste animi earum incidunt similique eos, amet perferendis quidem dolorum numquam. Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint iusto quia laboriosam hic vero, ad fuga nihil cumque! Perferendis fugiat atque voluptate non voluptatum ipsum, magnam cumque reprehenderit dolore nulla.
        </p>
        
        <p class="article-p">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum tempora error ab? Recusandae distinctio optio omnis alias ea labore voluptatem architecto similique minima velit, numquam maxime eum enim reprehenderit ducimus. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facere accusamus esse quas soluta quod, ab eligendi in! Nesciunt quasi velit ipsam eius veritatis non itaque et quidem, ipsa, esse odio. Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati deleniti ea aliquam fuga quam iure excepturi, cum natus incidunt ducimus, eveniet voluptatum. Esse saepe doloribus facilis est voluptas placeat voluptatibus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, deleniti odit? Corrupti, nihil, illum dolorum eveniet itaque earum a sed nostrum, odit autem quod quam accusamus qui. Blanditiis, reiciendis neque.
        </p>

    </Article>
</div>