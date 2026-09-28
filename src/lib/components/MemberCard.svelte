<script>
    let {
        name = "Firstname Lastname",
    } = $props();
</script>

<div class="flex p-5 bg-ac-light-yellow w-1/4 rounded-3xl border-3 border-ac-white text-center justify-center place-content-center">
    <div class="bg-ac-pink rounded-full w-20 h-20"> </div>
    <p class="pl-5 text-center justify-center place-content-center"> {name} </p>
</div>