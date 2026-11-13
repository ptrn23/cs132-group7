<script>
    import Overview from "$lib/sections/Overview.svelte";
    import ResearchQuestions from "$lib/sections/ResearchQuestions.svelte";
    import DataCollection from "$lib/sections/DataCollection.svelte";
    import EDA from "$lib/sections/EDA.svelte";

    import karin from "$lib/assets/karin.png";
    import lej from "$lib/assets/lej.jpg";
    import paul from "$lib/assets/paul.jpeg";
    import marco from "$lib/assets/marco.jpg";

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
            <MemberCard name="Marco Cantero" title="Hungry" birthday="Jul 4" pic={marco} desc="curious CS student interested in AI and collector of many hobbies!" linkedin="https://www.linkedin.com/in/marcocantero/"/>
            <MemberCard name="Carlyne Consebido" title="Overcaffeinated" birthday="Apr 21" pic={karin} desc="just a lil silly sometimes" linkedin="https://www.linkedin.com/in/carlyne-consebido/"/>
        </div>
        <div class="flex gap-x-5">
            <MemberCard name="Lejand Errol Coralde" title="Skinny Legend" birthday="May 28" pic={lej} desc="Best in Tulog. Best in LARP. Best in Sudoku. Best in Table Tennis. Best in Hairstyling... and Best student ng CVMIL :>>" linkedin="https://www.linkedin.com/in/lejand-errol-coralde/" github="https://github.com/Lejaaand"/>
            <MemberCard name="Paul Timothy Necasio" title="Now playing..." birthday="Feb 23" pic={paul} desc="hello! i’m paul :) i’m interested in web and game development, alongside my hobby of graphic design. " linkedin="https://www.linkedin.com/in/paul-timothy-necasio-626a68152/" github="https://github.com/ptrn23" bsky="https://bsky.app/profile/ptrn23.bsky.social"/>
        </div>
    </section>
</div>