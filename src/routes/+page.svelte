<script>
    import Card from "$lib/components/Card.svelte";
    import MemberCard from "$lib/components/MemberCard.svelte";
    import CardWithTitle from "$lib/components/CardWithTitle.svelte";

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
    
    <section id="data">
        <p class="text-xl font-bold"> Data Collection </p>
        <p class="font-semibold"> Dataset Description </p>
        <p class=""> This project will use two types of datasets: </p>
        <ul class="list-disc pl-8 pb-2">
            <li> retail prices dataset (tracking absolute ₱/kg for Cereals, Rootcrops, Fruits, Leafy Vegetables, and Fruit Vegetables) </li>
            <li> Consumer Price Index dataset (tracking inflation indices for Bottom 30% and All Income households) </li>
        </ul>

        <p class="font-semibold"> Data Collection Process </p>
        <p> All data was acquired through OpenStat, the open data portal managed by the Philippine Statistics Authority (PSA). </p>

        <p class="pl-2"> Calorie-dense Food </p>
        <ol class="list-decimal pl-8 pb-2"> 
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__2018NEW/0042M4ARN01.px/?rxid=b030d5e8-77f7-488c-bb2a-ec0aec32d59a"> Cereals: Retail Prices of Agricultural Commodities by Geolocation, Commodity, Year and Period </a> </li>
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__2018NEW/0042M4ARN02.px/?rxid=b030d5e8-77f7-488c-bb2a-ec0aec32d59a" >Rootcrops: Retail Prices of Agricultural Commodities by Geolocation, Commodity, Year and Period </a> </li>
        </ol>

        <p class="pl-2"> Nutrient-dense Food </p>
        <ol class="list-decimal pl-8 pb-2"> 
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__2018NEW/0042M4ARN05.px/?rxid=b030d5e8-77f7-488c-bb2a-ec0aec32d59a"> Fruit Vegetables: Retail Prices of Agricultural Commodities by Geolocation, Commodity, Year and Period </a> </li>
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__2018NEW/0042M4ARN06.px/?rxid=b030d5e8-77f7-488c-bb2a-ec0aec32d59a"> Leafy Vegetables: Retail Prices of Agricultural Commodities by Geolocation, Commodity, Year and Period </a> </li>
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__2018NEW/0042M4ARN07.px/?rxid=b030d5e8-77f7-488c-bb2a-ec0aec32d59a"> Fruits: Retail Prices of Agricultural Commodities by Geolocation, Commodity, Year and Period </a> </li>
        </ol>

        <p class="pl-2"> Consumer Price Index </p>
        <ol class="list-decimal pl-8 pb-2">
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__PI__BIH__2018NEW/0022M4ABIR1.px/?rxid=9ac08fde-3be2-4941-8b85-0a12242bb764"> Consumer Price Index for Bottom 30% Income Households by Commodity Group (2018=100): January 2018 - August 2026 </a> </li>
            <li> <a class="text-blue-500 underline" href="https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__PI__CPI__2018NEW/0012M4ACP22.px/?rxid=cf799e95-a36e-4896-b860-e6412f6b3108"> Consumer Price Index for All Income Households by Commodity Group (2018=100): January 2018 - August 2026 </a> </li>
        </ol>

        <p class="font-semibold"> Sampling Method </p>
        <p> The PSA conducts and collects all national censuses and surveys for their data. For this project, we isolated the scope of the datasets to cover specific food groups and to only cover the NCR. </p>

        <p class="font-semibold"> Data set size </p>
        <p> Before preprocessing </p>
        <ul class="list-disc pb-2 pl-8"> 
            <li> Date: January 2018 - August 2026 (monthly) </li>
            <li> Region: 120 regional areas in the Philippines (including Philippines, cities, and provinces) </li>
            <li> <p> Retail Prices dataset </p>
                <ul class="list-disc pl-8"> 
                    <li> 5 datasets (Fruits, Fruit Vegetables, Leafy Vegetables, Cereals, Rootcrops) </li>
                    <li> 4284 + 1071 + 1428 + 1666 + 2975 rows (respectively) = 11424 rows in total </li>
                </ul>
            </li>
            <li> <p> Consumer Price Index dataset </p>
                <ul class="list-disc pl-8"> 
                    <li> 2 datasets (Bottom 30% Income, All Income) </li>
                    <li> 37680 + 42480 rows (respectively) = 80160 rows in total </li>
                    <li> 354 commodities (includes food, financial services, education, furniture, etc.) </li>
                </ul>
            </li>
        </ul>

        <p> After preprocessing </p>
        <ul class="list-disc pb-3 pl-8"> 
            <li> Date: January 2020 - August 2026 (monthly) </li>
            <li> Region: National Capital Region (NCR) </li>
            <li> <p> Retail Prices dataset </p>
                <ul class="list-disc pl-8"> 
                    <li> 1884 rows </li>
                    <li> 2 major groups (nutrient-dense vs. calorie-dense) </li>
                    <li> 5 subgroups (Fruits, Fruit Vegetables, Leafy Vegetables, Cereals, Rootcrops) </li>
                    <li> 80 months per commodity </li>
                </ul>
            </li>
            <li> <p> Consumer Price Index dataset </p>
                <ul class="list-disc pl-8"> 
                    <li> 960 rows </li>
                    <li> 2 major groups (Bottom 30% Income, All Income) </li>
                    <li> 80 months per commodity </li>
                </ul>
            </li>
        </ul>

        <p class="font-semibold"> Preprocessing </p>
        <p> Preprocessing for retail prices dataset </p>
        <ol class="list-decimal pl-8">
            <li> filter the Geolocation column to be ..NCR - National Capital Region only </li>
            <li> drop the columns for 2018 January to 2019 Annual </li>
            <li> drop the columns for 2026 September to 2026 Annual </li>
            <li> drop the columns for 2020 Annual, 2021 Annual, 2022 Annual, 2023 Annual, 2024 Annual, 2025 Annual </li>
            <li> convert the month-year columns into rows </li>
            <li> convert the month-year rows into proper datetime </li>
            <li> include a column and categorize all food groups (while categorizing by the 5 types)</li>
        </ol>
        <p> Sample Data </p>
            <div class="ml-8 mb-5 shadow-xs rounded-base border border-default w-2/3">
                <table class="w-full text-sm text-left">
                    <thead class="text-sm text-body border-b rounded-base border-default">
                        <tr>
                            <th scope="col" class="px-6 py-3 font-medium">
                                date
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                food_type
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                sub_category
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                commodity
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                price
                            </th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr class="bg-neutral-primary border-b border-default">
                            <th scope="row" class="px-6 py-4">
                                2020-01-01
                            </th>
                            <td class="px-6 py-4">
                                Calorie-Dense
                            </td>
                            <td class="px-6 py-4">
                                Cereals
                            </td>
                            <td class="px-6 py-4">
                                RICE REGULAR MILLED, 1 KG
                            </td>
                            <td class="px-6 py-4">
                                38.50
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>

        <p> Preprocessing for Consumer Price Index dataset </p>
        <ol class="list-decimal pl-8">
            <li> filter the Geolocation column to be NCR only </li>
            <li> drop the columns for 2018 Jan to 2019 Ave </li>
            <li> drop the columns for 2026 Sep to 2026 Ave </li>
            <li> drop the columns for 2020 Ave, 2021 Ave, 2022 Ave, 2023 Ave, 2024 Ave, 2025 Ave </li>
            <li> filter the rows for these: 
                <ol class="list-decimal pl-8"> 
                    <li> "0 - ALL ITEMS": baseline inflation </li>
                    <li> "01.1.1.1 - Cereals (ND)": cereals </li>
                    <li> "01.1.7.5 - Tubers, plantains and cooking bananas (ND)": rootcrops </li>
                    <li> "01.1.6 - Fruits and nuts (ND)": fruits </li>
                    <li> "01.1.7.1 - Leafy or stem vegetables, fresh or chilled (ND)": leafy vegetables </li>
                    <li> "01.1.7.2 - Fruit-bearing vegetables, fresh or chilled (ND)": fruit vegetables </li>
                </ol>
            </li>
            <li> convert the month-year columns into rows </li>
            <li> convert the month-year rows into proper datetime </li>
        </ol>

        <p> Sample Data </p>
            <div class="ml-8 shadow-xs rounded-base border border-default w-2/3">
                <table class="w-full text-sm text-left">
                    <thead class="text-sm text-body border-b rounded-base border-default">
                        <tr>
                            <th scope="col" class="px-6 py-3 font-medium">
                                date
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                income_group
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                food_type
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                sub_category
                            </th>
                            <th scope="col" class="px-6 py-3 font-medium">
                                cpi
                            </th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr class="bg-neutral-primary border-b border-default">
                            <th scope="row" class="px-6 py-4">
                                2020-01-01
                            </th>
                            <td class="px-6 py-4">
                                Bottom 30%
                            </td>
                            <td class="px-6 py-4">
                                Baseline
                            </td>
                            <td class="px-6 py-4">
                                ALL ITEMS
                            </td>
                            <td class="px-6 py-4">
                                105.2
                            </td>
                        </tr>

                        <tr class="bg-neutral-primary border-b border-default">
                            <th scope="row" class="px-6 py-4">
                                2020-01-01
                            </th>
                            <td class="px-6 py-4">
                                All Income
                            </td>
                            <td class="px-6 py-4">
                                Nutrient-Dense
                            </td>
                            <td class="px-6 py-4">
                                Fruits
                            </td>
                            <td class="px-6 py-4">
                                108.4
                            </td>
                        </tr>

                        <tr class="bg-neutral-primary border-b border-default">
                            <th scope="row" class="px-6 py-4">
                                2020-01-01
                            </th>
                            <td class="px-6 py-4">
                                Bottom 30%
                            </td>
                            <td class="px-6 py-4">
                                Calorie-Dense
                            </td>
                            <td class="px-6 py-4">
                                Cereals
                            </td>
                            <td class="px-6 py-4">
                                102.1
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>

    <p class="font-semibold"> Preprocessed Datasets </p>
    <p> <a class="text-blue-500 underline" href="https://docs.google.com/spreadsheets/d/17t6uVtI6CKeNMy7MRdKvYsVFrtNgjwn9CcHiKXYWtBY/edit?usp=drive_link"> Retail Prices Dataset </a></p>
    <p> <a class="text-blue-500 underline" href="https://docs.google.com/spreadsheets/d/1R6nCpYbEkWRNtuBCi6Wzraem0R9GwkXNetu9Vd-Yr28/edit?usp=drive_link"> CPI Dataset </a> </p>
    </section>
</div>