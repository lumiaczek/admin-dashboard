<script>
    import SubscriptionItem from "./SubscriptionItem.svelte";
    import SubscriptionValue from "./SubscriptionValue.svelte";
</script>

<div class="grid grid-cols-1 lg:grid-cols-3 gap-5 text-center">
    <SubscriptionItem title={"Darmowy"}>
        <ul>
            <SubscriptionValue text={"Pomoc społeczności"}/>
            <SubscriptionValue text={"500 produktów w bazie"}/>
            <SubscriptionValue text={"Ręczne kopie zapasowe"}/>
        </ul>
    </SubscriptionItem>

    <SubscriptionItem title={"Rozszerzony"}>
        <ul>
            <SubscriptionValue text={"Pomoc w ciągu 24 godzin"}/>
            <SubscriptionValue text={"1500 produktów w bazie"}/>
            <SubscriptionValue text={"1 automatyczna kopia zapasowa"}/>
        </ul>
    </SubscriptionItem>

    <SubscriptionItem title={"PRO"}>
        <ul>
            <SubscriptionValue text={"Pomoc w ciągu 1 godziny"}/>
            <SubscriptionValue text={"∞ produktów w bazie"}/>
            <SubscriptionValue text={"Automatyczne kopie zapasowe"}/>
        </ul>
    </SubscriptionItem>
</div>