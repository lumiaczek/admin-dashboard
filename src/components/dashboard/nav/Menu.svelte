<script>
    import MenuItem from "./MenuItem.svelte";
    import Modal from "../../utils/Modal.svelte";
    import Subscription from "../subscription/Subscription.svelte";
</script>

<ul>
    <MenuItem name={"Panel główny"} url={"/admin"}/>
    <MenuItem name={"Kalendarz"} url={"/admin/calendar"}/>
    <MenuItem name={"Tabela danych"} url={"/admin/table"}/>
    <MenuItem name={"Galeria"} url={"/admin/gallery"}/>
    <MenuItem name={"Regulamin"} url={"/admin/regulation"}/>
    <MenuItem name={"FAQ"} url={"/admin/faq"}/>
    <MenuItem name={"Kontakt"} url={"/admin/contact"}/>

    <Modal buttonTitle={"Usługi dodatkowe"} title={"Wybierz pakiet usług dodatkowych, który  ci odpowiada"}>
        <Subscription/>
    </Modal>
</ul>