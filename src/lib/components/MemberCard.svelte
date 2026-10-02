<script>
    let {
        name = "Firstname Lastname",
    } = $props();
</script>

<div class="flex p-5 bg-ac-light-yellow w-1/4 rounded-3xl border-3 border-ac-white text-center justify-center place-content-center">
    <p class="pl-5 text-center font-semibold justify-center place-content-center"> {name} </p>
</div>