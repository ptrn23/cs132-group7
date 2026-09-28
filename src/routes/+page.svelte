<script>
    import Card from "$lib/components/Card.svelte";
    import MemberCard from "$lib/components/MemberCard.svelte";
</script>

<div class="px-10 py-5 text-ac-dark-brown">
    <section id="overview" class="pb-5">
        <p class="text-4xl font-bold"> Health is Wealth </p>
        <p class="text-xl font-semibold pb-3"> Analyzing the Affordability of Nutrient-Dense Foods Against the Inflation Inequality in the National Capital Region (2020-2026) </p>
    
        <div class="flex gap-x-5">
            <MemberCard />
            <MemberCard />
            <MemberCard />
            <MemberCard />
        </div>
    </section>

    <section id="" class="pb-5 flex">
        <div class="w-2/5 pr-5">
            <p class="text-xl font-semibold pb-3"> Overview </p>
            <p> Being able to afford a healthy diet should be a universal right, and not a privilege. However, due to food price inflation, healthy foods have become less and less affordable, particularly for low-income households. This issue has only worsened due to the COVID-19 pandemic, further highlighting the disparities in access to nutritious food. </p>
        </div>

        <div class="w-3/5">
            <p class="text-xl font-semibold pb-3"> Problem </p>
            <p class="pb-5"> Nutrient-dense foods have become less affordable throughout the years; prices have gone up faster than wages, contributing to inflation inequality. This creates a heavier burden for low-income households, making healthy diets inaccessible. </p>

            <p class="text-xl font-semibold pb-3"> Solution </p>
            <p> This study aims to use data science to quantify the affordability of nutrient-dense foods throughout the years. In particular, we will compare the trends of food prices against the consumer price index of households in NCR. </p>
        </div>
    </section>
    
    <p class="text-xl font-semibold"> Objectives </p>
    <div class="flex gap-5 pb-5"> 
        <Card />
        <Card />
        <Card />
    </div>

    <p class="text-xl font-semibold"> Research Questions </p>
    <div class="flex gap-5 pb-5"> 
        <Card text="How do the absolute retail prices (₱/kg) and inflation rates of plant-based nutrient-dense foods (fruits, leafy vegetables, fruit vegetables) compare to calorie-dense foods (cereals, rootcrops) in the NCR from 2020 to 2026?"/>
        <Card text="How does the food-specific consumer price inflation for the Bottom 30% Income Households compare to All Income Households?"/>
        <Card text="What is the “affordability gap” ratio between nutrient-dense produce and calorie-dense staples, and how has this nutritional “price penalty” evolved?"/>
    </div>

    <p class="text-xl font-semibold"> Research Hypothesis </p>
    <div class="flex gap-5 pb-5"> 
        <Card />
        <Card />
        <Card />
    </div>

    <p class="text-xl font-semibold"> Data Collection </p>
</div>