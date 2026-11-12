<script>
    import Overview from "$lib/sections/Overview.svelte";
    import ResearchQuestions from "$lib/sections/ResearchQuestions.svelte";
    import DataCollection from "$lib/sections/DataCollection.svelte";

    import MemberCard from "$lib/components/MemberCard.svelte";

    import RQ2 from "$lib/assets/rq2_inflation_gap.png";
    import RQ3 from "$lib/assets/rq3_affordability_ratio.png";
    import Nutshell from "$lib/assets/nutshell.png";
</script>

<!-- TODO: components per section -->
<div class="px-20 py-5 text-ac-dark-brown">
    <Overview />
    <ResearchQuestions />
    <DataCollection />

    <section id="eda" class="pt-5 pb-5">
        <p class="text-xl font-bold pb-3"> Exploratory Data Analysis </p>

        <div>
            <img src={RQ2} alt="Research Question 2"/>
            <img src={RQ3} alt="Research Question 3"/>
            <img src={Nutshell} alt="Nutshell Plot"/>
        </div>
    </section>

    <section id="about">
        <p class="text-xl font-bold pb-3"> About Us </p>
        <div class="flex gap-x-5">
            <MemberCard name="Marco Cantero"/>
            <MemberCard name="Carlyne Consebido"/>
            <MemberCard name="Lejand Errol Coralde"/>
            <MemberCard name="Paul Timothy Necasio"/>
        </div>
    </section>
</div>