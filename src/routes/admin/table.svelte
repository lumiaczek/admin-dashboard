<script>
    import TableWrapper from "../../components/table/TableWrapper.svelte";
    import Th from "../../components/table/Th.svelte";
    import Td from "../../components/table/Td.svelte";
    import BreadcrumbsItem from "../../components/utils/BreadcrumbsItem.svelte";

</script>

<main>
    <div class="bg-blue-100 shadow rounded mb-4 p-4 flex justify-start items-center truncate">
        <BreadcrumbsItem url={"/"}>
            <i class="fa-solid fa-house text-2xl"></i>
        </BreadcrumbsItem>
        <BreadcrumbsItem url={"/admin"} class={"text-gray-500"}>
            <span class="ml-2">
                Panel Administracyjny
            </span>
        </BreadcrumbsItem>
        <BreadcrumbsItem url={"/table"} isCurrent={true}>
            <span class="ml-2">
                Lista Użytkowników
            </span>
        </BreadcrumbsItem>
    </div>
    <TableWrapper>
        <thead>
            <tr>
                <Th>
                    Imię
                </Th>
                <Th>
                    Nazwisko
                </Th>
                <Th>
                    Adres e-mail
                </Th>
                <Th>
                    Telefon
                </Th>
                <Th>
                    Data rejestracji
                </Th>
                <Th/>
            </tr>
        </thead>
        <tbody>
            <tr>
                <Td>
                    Daniel
                </Td>
                <Td>
                    Borowski
                </Td>
                <Td>
                    danielborowski05@gmail.com
                </Td>
                <Td>
                    123-456-789
                </Td>
                <Td>
                    29 lipca 2022
                </Td>
                <Td class={"td-actions"}>
                    <a href="/" class="btn btn-info">
                        Zobacz
                    </a>
                </Td>
            </tr>
            <tr>
                <Td>
                    Adam
                </Td>
                <Td>
                    Winiarski
                </Td>
                <Td>
                    example@mail.com
                </Td>
                <Td>
                    123-456-789
                </Td>
                <Td>
                    29 lipca 2022
                </Td>
                <Td class={"td-actions"}>
                    <a href="/" class="btn btn-info">
                        Zobacz
                    </a>
                </Td>
            </tr>
            <tr>
                <Td>
                    Jan
                </Td>
                <Td>
                    Nowak
                </Td>
                <Td>
                    example@mail.com
                </Td>
                <Td>
                    123-456-789
                </Td>
                <Td>
                    29 lipca 2022
                </Td>
                <Td class={"td-actions"}>
                    <a href="/" class="btn btn-info">
                        Zobacz
                    </a>
                </Td>
            </tr>
            <tr>
                <Td>
                    Natalia
                </Td>
                <Td>
                    Lewandowska
                </Td>
                <Td>
                    example@mail.com
                </Td>
                <Td>
                    123-456-789
                </Td>
                <Td>
                    29 lipca 2022
                </Td>
                <Td class={"td-actions"}>
                    <a href="/" class="btn btn-info">
                        Zobacz
                    </a>
                </Td>
            </tr>
        </tbody>
    </TableWrapper>

    
</main>