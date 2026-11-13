<script>
    import Linkedin from "$lib/assets/linkedin.png";
    import Bluesky from "$lib/assets/bsky.png";
    import Github from "$lib/assets/github.png";

    let {
        name = "Firstname Lastname",
        title = "Title",
        birthday = "Jan 1",
        desc = "Lorem ipsum dolor",
        pic = "",
        linkedin = "",
        bsky ="",
        github = ""
    } = $props();
</script>

<div class="flex p-10 px-15 bg-ac-light-brown w-1/2 rounded-3xl border-b-3 border-ac-brown">
    <img src={pic} alt="img" class="w-35 h-35 rounded-lg border-3 border-ac-cream"/>

    <div class="relative flex flex-col">
        <p class="pl-5 font-bold text-lg"> {name} </p>
        <p class="pl-5 italic"> {title} </p>
        <p class="pl-5"> Born {birthday} </p>
        <p class="pl-5 pb-2 text-sm"> {desc} </p>

        <div class="flex ml-5 gap-x-2 mt-auto">
            <a href={linkedin}> <img src={Linkedin} alt="linkedin" class="h-5 w-5" /> </a>
            {#if github}
                <a href={github}> <img src={Github} alt="github" class="h-5 w-5" /> </a>
            {/if}
            {#if bsky}
                <a href={bsky}> <img src={Bluesky} alt="bluesky" class="h-5 w-5" /> </a>
            {/if}
        </div>
        
    </div>
</div>