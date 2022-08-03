<script>
    import Card from "../../utils/Card.svelte";
    import Button from "../../utils/Button.svelte";
    export let title = '';
</script>

<div>
    <Card class={"group transition hover:shadow-2xl hover:scale-105 hover:bg-blue-100"} title={title}>
        <Card>
            <slot></slot>
        </Card>
        <div class="mb-3"></div>
        <Button className={"primary"} klasa={"w-full flex justify-center"} >
            <i class="fa-solid fa-circle-check text-md"></i>
            <span class="ml-2">
                Wybierz
            </span>
        </Button>
    </Card>
</div>