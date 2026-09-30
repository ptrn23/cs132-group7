<script>
    import Card from "$lib/components/Card.svelte";
    import MemberCard from "$lib/components/MemberCard.svelte";

    import Two from "$lib/assets/zero_hunger.png";
    import Ten from "$lib/assets/red_ineq.png";
</script>

<div class="px-20 py-5 text-ac-dark-brown">
    <section id="overview" class="pb-5">
        <p class="text-4xl font-bold"> Health is Wealth </p>
        <p class="text-xl font-semibold pb-3"> Analyzing the Affordability of Nutrient-Dense Foods Against the Inflation Inequality in the National Capital Region (2020-2026) </p>
    
        <div class="flex gap-x-5">
            <MemberCard name="Marco Cantero"/>
            <MemberCard name="Carlyne Consebido"/>
            <MemberCard name="Lejand Errol Coralde"/>
            <MemberCard name="Paul Timothy Necasio"/>
        </div>
    </section>

    <section id="" class="pb-5 flex">
        <div class="w-3/5 pr-5">
            <p class="text-xl font-bold pb-3"> Overview </p>
            <p class="pb-2"> Being able to afford a healthy diet should be a universal right, and not a privilege. However, due to food price inflation, healthy foods have become less and less affordable, particularly for low-income households. This issue has only worsened due to the COVID-19 pandemic, further highlighting the disparities in access to nutritious food. This is especially apparent in the National Capital Region (NCR), where the cost of living is among the highest in the Philippines. With this, valuable insights can be obtained from examining the relationship between food prices and how much different households spend on average on consumer goods. </p>
        
            <div class="flex justify-center gap-x-5">
                <img src={Two} alt="Zero Hunger" class="w-40 h-40 rounded-xl"/>
                <img src={Ten} alt="Reduced Inequalities" class="w-40 h-40 rounded-xl"/>
            </div>
        </div>

        <div class="w-2/5">
            <p class="text-xl font-bold pb-3"> Problem </p>
            <p class="pb-5"> Nutrient-dense foods have become less affordable throughout the years; prices have gone up faster than wages, contributing to inflation inequality. This creates a heavier burden for low-income households, making healthy diets inaccessible. </p>

            <p class="text-xl font-bold pb-3"> Solution </p>
            <p> This study aims to use data science to quantify the affordability of nutrient-dense foods throughout the years. In particular, we will compare the trends of food prices against the consumer price index of households in NCR, which refers to the average spendings of households on consumer goods, over time. </p>
        </div>
    </section>
    
    <section id="objectives">
        <p class="text-xl font-bold pb-2"> Objectives </p>
        <div class="flex gap-5 pb-5"> 
            <Card text="To analyze and compare the absolute retail prices and calculated inflation rates of nutrient-dense foods (fruits, vegetables) versus calorie-dense foods (rice, cereals)"/>
            <Card color="bg-ac-light-pink" text="To determine whether the rising prices of fresh produce unevenly affect food accessibility and affordability among Bottom 30% Income Households compared with the rest of All Income Households"/>
            <Card text="To quantify the nutritional “price penalty” by modeling the ratio of nutrient-dense food prices to calorie-dense staple prices"/>
        </div>
    </section>
    
    <section id="questions">
        <p class="text-xl font-bold pb-2"> Research Questions </p>
        <div class="flex gap-5 pb-5"> 
            <Card color="bg-ac-light-pink" text="How do the absolute retail prices (₱/kg) and inflation rates of plant-based nutrient-dense foods (fruits, leafy vegetables, fruit vegetables) compare to calorie-dense foods (cereals, rootcrops) in the NCR from 2020 to 2026?"/>
            <Card text="How does the food-specific consumer price inflation for the Bottom 30% Income Households compare to All Income Households?"/>
            <Card color="bg-ac-light-pink" text="What is the “affordability gap” ratio between nutrient-dense produce and calorie-dense staples, and how has this nutritional “price penalty” evolved?"/>
        </div>
    </section>
    
    <section id="hypothesis">
        <p class="text-xl font-bold pb-2"> Research Hypothesis </p>
        <div class="flex gap-5 pb-5"> 
            <Card text="The inflation rate and absolute price of nutrient-dense foods in the NCR are significantly higher than that of calorie-dense foods"/>
            <Card color="bg-ac-light-pink" text="Price increases of nutrient-dense foods have had a greater impact on food accessibility and affordability of Bottom 30% Income Households compared to the general population (All Income Households)"/>
            <Card text="The “affordability gap” ratio has continuously increased from 2020 to 2026, hence restricting access to nutrient-dense foods for the urban poor"/>
        </div>
    </section>
    
    <section id="data">
        <p class="text-xl font-bold"> Data Collection </p>
        <p class="font-medium"> Source: Philippine Statistics Authority (PSA) </p>
        <p class="pb-3"> This project will use two types of datasets: retail prices of agricultural commodities and consumer price index of households.</p>

        <p class="font-semibold pb-2"> Retail Prices of Agricultural Commodities </p>
        <p> These datasets concern the retail prices by Geolocation and Specific Commodity over time of Nutrient-dense Foods (Fruit Vegetables, Leaf Vegetables, Fruits) and Calorie-dense Foods (Cereals, Rootcrops).  </p>
    
        <p class="font-semibold pb-2"> Consumer Price Index </p>
        <p> </p>
    </section>
</div>