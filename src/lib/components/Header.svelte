<script>
    // const headers = [
    //     { label: 'Home', url: '/' },
    //     { label: 'Overview', url: '#overview' }, 
    //     { label: 'Data', url: '#data' },
    //     { label: 'Method', url: '#method' },
    //     { label: 'Results', url: '#results' },
    //     { label: 'Conclusion', url: '#conclusion' },
    //     { label: 'About Us', url: '#about' },
    // ]

    const headers = [
        { label: 'Overview', url: '#overview'},
        { label: 'Objectives', url: '#objectives'},
        { label: 'Questions', url: '#questions'},
        { label: 'Hypothesis', url: '#hypothesis'},
        { label: 'Data Collection', url: '#data'},
    ];
</script>

<div class="bg-ac-light-pink rounded-bl-[300%_200%] rounded-br-[300%_200%] shadow-[rgba(0,0,0,0.8)_0px_0px_16px_0px] flex flex-col h-25 justify-around left-0 pb-[60px] pl-[60px] pr-[60px] pt-[30px] right-3 top-0 w-full z-50">
    <div class="flex gap-10 justify-center">
        {#each headers as header}
            <div class="px-5 py-2 rounded-xl hover:bg-ac-pink">
                <a class="text-xl text-ac-dark-brown font-bold" href={header.url}> {header.label} </a>
            </div>
        {/each}
    </div>
</div>