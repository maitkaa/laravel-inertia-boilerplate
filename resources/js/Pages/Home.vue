<template>
        <div class='flex items-center justify-center min-h-screen'>
            <div class="bg-slate-800 h-screen w-screen">
                <div class="bg-slate-700 shadow-md rounded rounded-xl m-16 border border-indigo-500/50 shadow-xl shadow-indigo-500/50 relative inset-y-1/4">
                    <div class="flex flex-col p-10  px-16 space-y-6 items-center text-center">
                        <h1 class="font-light md:text-6xl text-5xl text-white tracking-wide ">Boilerplate with <span id="spin" class="text-transparent font-normal bg-clip-text bg-gradient-to-r from-indigo-400 to-cyan-300 leading-[5rem] "></span> <br/> Build something awesome </h1>
                        <p class="text-gray-400 md:text-2xl text-xl px-18"> {{ info }}</p>
                        <inertia-link class="rounded-full bg-indigo-500 shadow-lg shadow-indigo-500/50 text-white text-lg py-4 px-6" href="/demo">Inertia test</inertia-link>
                    </div>
                </div>
            </div>
        </div>
</template>
<script>
export default {
    setup: () => ({
        info: 'Button will demonstrate inertia page load.'
    })
}
</script>
<style scoped>
#spin {

}
#spin:after {
    content:"";
    animation: spin 10s linear infinite;
}
@keyframes spin {
    0% { content:"Laravel 9";}
    25% { content:"inertiaJs";}
    50% { content:"Vue 3";}
    75% { content:"Tailwind Css";}
    100% { content:"";}
}
</style>
