<script>
    import RQ1 from "$lib/assets/rq1.png";
    import RQ2 from "$lib/assets/rq2.png";
    import RQ3 from "$lib/assets/rq3.png";
    import Nutshell from "$lib/assets/nutshell_light.png";
</script>

<section id="eda" class="pb-5">
    <p class="text-xl font-bold mb-3 py-1.5 w-1/4 text-center px-4 bg-ac-light-pink rounded-full"> Exploratory Data Analysis </p>

    <div>
        <p class="text-lg font-semibold pb-3"> Research Question 1: Absolute Retail Prices </p>
        <div class="flex">
            <div class="w-1/3 pr-5 text-center justify-center place-content-center">
                <div class="mb-5 border rounded-lg border-3 p-5 border-ac-light-pink">
                    <p class="font-semibold"> Distribution Check (Shapiro-Wilk)</p>
                    <p class="text-lg"> 0.0839 & 0.0674 </p>
                    <p class="pb-2"> both > 0.05, <span class="text-green-600 font-bold"> NORMAL! </span> </p>

                    <p> Statistical Test: <span class="font-bold"> Independent T-test </span> </p>
                    <p> p-value = 0.2052 </p>
                    <p> > 0.05, <span class="text-red-600 font-bold"> FAIL TO REJECT NULL! </span> </p>
                </div>
                
                <div class="rounded-lg p-5 bg-ac-turquoise">
                    <p class="text-ac-white font-bold"> The inflation rate and absolute price of nutrient-dense foods in the NCR is not higher than that of calorie-dense foods (≤) </p>
                </div>
            </div>

            <div class="w-2/3">
                <img src={RQ1} alt="Research Question 1" class="rounded-lg pb-3"/>
            </div>
        </div>

        <p class="text-lg font-semibold pb-3"> Research Question 2: Consumer Price Index </p>
        <div class="flex">
            <div class="w-1/3 pr-5 text-center justify-center place-content-center">
                <div class="mb-5 border rounded-lg border-3 p-5 border-ac-light-pink">
                    <p class="font-semibold"> Distribution Check (Shapiro-Wilk)</p>
                    <p class="text-lg"> 2.6891e<sup>-0.4</sup> & 2.9620e<sup>-0.5</sup> </p>
                    <p class="pb-2"> both > 0.05, <span class="text-red-600 font-bold"> NON-NORMAL! </span> </p>

                    <p> Statistical Test: <span class="font-bold"> Wilcoxon Signed-Rank Test </span> </p>
                    <p> p-value = 6.2436e<sup>-0.6</sup> </p>
                    <p> &lt; 0.05, <span class="text-green-600 font-bold"> REJECT NULL! </span> </p>
                </div>
                
                <div class="rounded-lg p-5 bg-ac-turquoise">
                    <p class="text-ac-white font-bold"> Price increases of nutrient-dense foods have had a greater impact on the food accessibility and affordability of Bottom 30% Income Households than on All Income Households (>) </p>
                </div>
            </div>

            <div class="w-2/3">
                <img src={RQ2} alt="Research Question 2" class="rounded-lg pb-3"/>
            </div>
        </div>

        <p class="text-lg font-semibold pb-3"> Research Question 3: Affordability Ratio </p>
        <div class="flex">
            <div class="w-1/3 pr-5 text-center justify-center place-content-center">
                <div class="mb-5 border rounded-lg border-3 p-5 border-ac-light-pink">
                    <p> Statistical Test: <span class="font-bold"> Linear Regression </span> </p>
                    <p> p-value = 4.1786e<sup>-0.7</sup> </p>
                    <p> &lt; 0.05, <span class="text-green-600 font-bold"> REJECT NULL! </span> </p>
                </div>
                
                <div class="rounded-lg p-5 bg-ac-turquoise">
                    <p class="text-ac-white font-bold"> The affordability gap ratio has increased from 2020 to 2026, so there is evidence of restricted access to nutrient-dense foods for the urban poor (>). </p>
                </div>
            </div>

            <div class="w-2/3">
                <img src={RQ3} alt="Research Question 3" class="rounded-lg pb-3"/>
            </div>
        </div>

        <p class="text-lg font-semibold pb-3"> In A Nutshell </p>
        <img src={Nutshell} alt="Nutshell Plot" class="rounded-lg pb-3"/>
    </div>
</section>