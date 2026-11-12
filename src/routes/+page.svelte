<script>
    import Overview from "$lib/sections/Overview.svelte";
    import ResearchQuestions from "$lib/sections/ResearchQuestions.svelte";
    import DataCollection from "$lib/sections/DataCollection.svelte";
    import EDA from "$lib/sections/EDA.svelte";

    import MemberCard from "$lib/components/MemberCard.svelte";
    import Divider from "$lib/components/Divider.svelte";
</script>

<div class="px-20 py-5 text-ac-dark-brown">
    <Overview />
    <Divider />
    <ResearchQuestions />
    <Divider />
    <DataCollection />
    <Divider />
    <EDA />
    <Divider />

    <section id="about">
        <p class="text-xl font-bold mb-3 py-1.5 w-1/8 text-center px-4 bg-ac-light-pink rounded-full"> About Us </p>
        <div class="flex gap-x-5 pb-3">
            <MemberCard name="Marco Cantero"/>
            <MemberCard name="Carlyne Consebido" title="Overcaffeinated" birthday="Apr 21"/>
        </div>
        <div class="flex gap-x-5">
            <MemberCard name="Lejand Errol Coralde"/>
            <MemberCard name="Paul Timothy Necasio"/>
        </div>
    </section>
</div>