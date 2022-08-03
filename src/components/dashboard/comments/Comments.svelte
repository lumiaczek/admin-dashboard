<script>
    import Card from "../../utils/Card.svelte";
    import Comment from "./Comment.svelte";
</script>

<Card title={"Najświeższe komentarze"}>
    <ul class="grid grid-cols-1 gap-2">
        <Comment tytul={"Komentarz przykładowy"} date="2021-08-15">
            Świetna obsługa! Wszystko tak, jak być należy.
        </Comment>

        <Comment tytul={"Komentarz przykładowy"} date="2021-08-15">
            Świetna obsługa! Wszystko tak, jak być należy.
        </Comment>

        <Comment tytul={"Komentarz przykładowy"} date="2021-08-15">
            Świetna obsługa! Wszystko tak, jak być należy.
        </Comment>

        <Comment tytul={"Komentarz przykładowy"} date="2021-08-15">
            Świetna obsługa! Wszystko tak, jak być należy.
        </Comment>
    </ul>
</Card>