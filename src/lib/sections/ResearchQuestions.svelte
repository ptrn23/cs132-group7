<script>
    import CardWithTitle from "$lib/components/CardWithTitle.svelte";
</script>

<section id="hypothesis">
    <p class="text-xl font-bold pb-2"> Research Questions and Hypotheses </p>

    <div class="flex gap-5 pb-3"> 
        <CardWithTitle title="How do the absolute retail prices (₱/kg) and inflation rates of plant-based nutrient-dense foods (fruits, leafy vegetables, fruit vegetables) compare to calorie-dense foods (cereals, rootcrops) in the NCR from 2020 to 2026?" text="" />
        <CardWithTitle title="Null Hypothesis" color="bg-none" text="There is no significant difference between the inflation rate and absolute price of nutrient-dense foods in NCR compared to that of calorie-dense foods"/>
        <CardWithTitle title="Alternative Hypothesis" color="bg-none" text="The inflation rate and absolute price of nutrient-dense foods in the NCR are significantly higher than that of calorie-dense foods"/>
    </div>

    <div class="flex gap-5 pb-3"> 
        <CardWithTitle color="bg-ac-light-pink" title="How does the food-specific consumer price inflation for the Bottom 30% Income Households compare to All Income Households?" text="" />
        <CardWithTitle title="Null Hypothesis" color="bg-none" text="Price increases of nutrient-dense foods have not had a significant difference in impact on food accessibility and affordability of Bottom 30% Income Households compared to All Income Households"/>
        <CardWithTitle title="Alternative Hypothesis" color="bg-none" text="Price increases of nutrient-dense foods have had a greater impact on food accessibility and affordability of Bottom 30% Income Households compared to the general population (All Income Households)"/>
    </div>

    <div class="flex gap-5 pb-5"> 
        <CardWithTitle title="What is the “affordability gap” ratio between nutrient-dense produce and calorie-dense staples, and how has this nutritional “price penalty” evolved?" text="" />
        <CardWithTitle title="Null Hypothesis" color="bg-none" text="The “affordability gap” ratio has not increased from 2020 to 2026"/>
        <CardWithTitle title="Alternative Hypothesis" color="bg-none" text="The “affordability gap” ratio has continuously increased from 2020 to 2026, hence restricting access to nutrient-dense foods for the urban poor"/>
    </div>
</section>