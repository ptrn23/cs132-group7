<script>
    let {
        name = "Firstname Lastname",
        title = "Title",
        birthday = "Jan 1",
        desc = "Lorem ipsum dolor"
    } = $props();
</script>

<div class="flex p-10 px-15 bg-ac-light-brown w-1/2 rounded-3xl border-b-3 border-ac-brown">
    <div class="bg-ac-light-pink w-30 h-30 rounded-lg self-start border-3 border-ac-cream">

    </div>

    <div class="">
        <p class="pl-5 font-bold text-lg"> {name} </p>
        <p class="pl-5 italic"> {title} </p>
        <p class="pl-5"> Born {birthday} </p>
        <p class="pl-5"> {desc} </p>
    </div>
</div>