<script>
    import Two from "$lib/assets/zero_hunger.png";
    import Ten from "$lib/assets/red_ineq.png";

    import Card from "$lib/components/Card.svelte";
</script>

<section id="overview" class="pb-5">
    <p class="text-4xl font-bold"> Health is Wealth </p>
    <p class="text-xl font-semibold pb-3"> Analyzing the Affordability of Nutrient-Dense Foods Against the Inflation Inequality in the National Capital Region (2020-2026) </p>
</section>

<section id="" class="pb-5 flex">
    <div class="w-2/5 pr-5">
        <p class="text-xl font-bold pb-3"> Overview </p>
        <p class="pb-3"> The Philippines, as an agricultural country, faces challenges regarding nutritional insecurity and economic disparity. Since the onset of the 2020 pandemic, food inflation has heavily impacted urban areas like the National Capital Region (NCR). While the common idea of inflation is frequently reported all over the news, there is a gap in understanding how this exact inflation affects markets and subsequently, how Filipinos choose to buy their food: do Filipinos struggle with weighing the price of nutrient-dense foods (e.g., fresh vegetables and fruits) versus calorie-dense staples (e.g., rice, rootcrops)? </p>
    
        <div class="flex justify-center gap-x-5">
            <img src={Two} alt="Zero Hunger" class="w-40 h-40 rounded-xl"/>
            <img src={Ten} alt="Reduced Inequalities" class="w-40 h-40 rounded-xl"/>
        </div>
    </div>

    <div class="w-3/5">
        <p class="text-xl font-bold pb-3"> Problem </p>
        <p class="pb-5"> Nutrient-dense foods have become less affordable throughout the years; prices have gone up faster than wages, contributing to inflation inequality. This creates a heavier burden for low-income households, making healthy diets inaccessible. </p>

        <p class="text-xl font-bold pb-3"> Solution </p>
        <p class="pb-2"> This study aims to use data science to quantify the affordability of nutrient-dense foods throughout the years. In particular, we will compare the trends of food prices against the consumer price index of households in NCR, which refers to the average spendings of households on consumer goods, over time. </p>
        <p> We will gather retail prices and Consumer Price Index (CPI) data, and then: </p>
        <ul class="list-disc pl-8 pb-2">
            <li> apply time-series analysis </li>
            <li> calculate inflation over time </li>
            <li> model affordability ratio </li>
        </ul>
        <p> The results of this study aim to raise awareness about food insecurity and help inform discussions on food assistance, nutrition programs, and other initiatives that aim to improve access to nutritious food. </p>
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