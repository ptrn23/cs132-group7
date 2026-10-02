<script>
    let {
        text = "text",
        color = "bg-ac-light-yellow"
    } = $props();
</script>

<div class="{`p-5 ${color} w-1/3 rounded-3xl border-3 border-ac-white text-center justify-center place-content-center`}">
    {text}
</div>