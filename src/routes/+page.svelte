<script>
    import Card from "$lib/components/Card.svelte";
</script>

<div class="px-10 py-5 text-ac-dark-brown">
    <p class="text-4xl font-bold"> Big Header </p>
    <p class="text-xl font-semibold"> Small Header </p>
    <p class="pb-5"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque nisl mi, dictum euismod sollicitudin eu, tempus ut sapien. Suspendisse sem enim, pellentesque eget pharetra ac, scelerisque quis ipsum. Nullam lobortis nisi dui, sed feugiat massa sollicitudin vel. Vivamus in massa vehicula, auctor mi sit amet, consectetur leo. Etiam mollis quam sit amet felis tincidunt tincidunt. Morbi efficitur, nibh vitae ornare maximus, mauris lectus lobortis ex, quis vulputate ante quam nec libero. Fusce porttitor ut sapien in varius. </p>

    <p class="text-xl font-semibold"> Research Questions </p>
    <div class="flex gap-5 pb-5"> 
        <Card text="How do the absolute retail prices (₱/kg) and inflation rates of plant-based nutrient-dense foods (fruits, leafy vegetables, fruit vegetables) compare to calorie-dense foods (cereals, rootcrops) in the NCR from 2020 to 2026?"/>
        <Card text="How does the food-specific consumer price inflation for the Bottom 30% Income Households compare to All Income Households?"/>
        <Card text="What is the “affordability gap” ratio between nutrient-dense produce and calorie-dense staples, and how has this nutritional “price penalty” evolved?"/>
    </div>
</div>