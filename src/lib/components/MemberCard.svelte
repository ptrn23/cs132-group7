<script>
    let {
        name = "Firstname Lastname",
        birthday = "Jan 1",
        desc = "Lorem ipsum dolor"
    } = $props();
</script>

<div class="flex p-10 px-15 bg-ac-light-green w-1/2 rounded-3xl border-3 border-ac-white">
    <div class="bg-ac-light-pink w-30 h-30 rounded-lg self-start">

    </div>

    <div class="">
        <p class="pl-5 font-bold"> {name} </p>
        <p class="pl-5"> {birthday} </p>
        <p class="pl-5"> {desc} </p>
    </div>
</div>