<script>
    import Card from "../../components/utils/Card.svelte";
    import AppStatus from "../../components/dashboard/status/AppStatus.svelte";
    import Newsletter from "../../components/dashboard/news/Newsletter.svelte";
    import Cta from "../../components/dashboard/cta/Cta.svelte";
    import Comments from "../../components/dashboard/comments/Comments.svelte";
import BreadcrumbsItem from "../../components/utils/BreadcrumbsItem.svelte";
</script>

<main class="overflow-x-hidden overflow-y-auto">
    <div class="bg-blue-100 shadow rounded mb-4 p-4 flex justify-start items-center truncate">
        <BreadcrumbsItem url={"/"}>
            <i class="fa-solid fa-house text-2xl"></i>
        </BreadcrumbsItem>
        <BreadcrumbsItem url={"/admin"} class={"text-gray-500"}>
            <span class="ml-2">
                Panel Administracyjny
            </span>
        </BreadcrumbsItem>
        <BreadcrumbsItem url={"/admin"} isCurrent={true}>
            <span class="ml-2">
                Panel Administracyjny
            </span>
        </BreadcrumbsItem>
    </div>
    <Card title={"Status"} class={"mb-4"}>
        <div class="w-full grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
            <AppStatus/>
        </div>
    </Card>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <section class="grid gap-4">
            <Newsletter 
                title={"Chcesz być na bieżąco?"} 
                subtitle={"Powiadomienia o naszych promocjach trafią bezpośrednio na Twoją skrzynke"}
            />
            <Cta 
                title={"Potrzebujesz pomocy eksperta?"} 
                subtitle={"Doradzimy, pomożemy!"} 
                call={"Skontaktuj się, z nami!"} 
                url = {"/admin/contact"}
            />
        </section>

        <Comments/>
    </div>
</main>