<script>
    import "../app.css";
    import { fade } from 'svelte/transition';
    import { base } from '$app/paths';

    function toggleNav() {
        const nav = document.getElementById("smallNav");
        if (!nav) return;
        nav.style.transform = nav.style.transform !== "scaleY(1)" ? "scaleY(1)" : "scaleY(0)";
    }

    export let data;
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300..700&family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap" rel="stylesheet">

<nav class="fixed top-0 left-0 right-0 z-50 flex items-center justify-between px-6 lg:px-10 py-4 bg-[#0a0a0a]/80 backdrop-blur-md border-b border-white/5">
    <a href="{base}/" class="font-mono font-semibold text-white hover:text-teal-400 transition-colors duration-200 text-base tracking-tight">
        Julian Jankowski
    </a>

    <!-- Desktop nav -->
    <div class="hidden lg:flex items-center gap-6">
        <a href="{base}/Projects" class="text-sm text-slate-400 hover:text-white transition-colors duration-200 tracking-wide">
            Projects
        </a>
        <a href="{base}/Socials" class="text-sm text-slate-400 hover:text-white transition-colors duration-200 tracking-wide">
            Socials
        </a>
        <div class="h-4 w-px bg-white/10 mx-1"></div>
        <a href="https://www.github.com/JulianJankowski" aria-label="GitHub" class="p-2 text-slate-400 hover:text-white hover:bg-white/5 rounded-lg transition-all duration-200">
            <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 24 24" fill="currentColor">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" />
            </svg>
        </a>
        <a href="https://www.linkedin.com/in/julian-jankowski-b1636b151/" aria-label="LinkedIn" class="p-2 text-slate-400 hover:text-white hover:bg-white/5 rounded-lg transition-all duration-200">
            <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" viewBox="0 0 256 256" fill="currentColor">
                <path d="M218.123122,218.127392 L180.191928,218.127392 L180.191928,158.724263 C180.191928,144.559023 179.939053,126.323993 160.463756,126.323993 C140.707926,126.323993 137.685284,141.757585 137.685284,157.692986 L137.685284,218.123441 L99.7540894,218.123441 L99.7540894,95.9665207 L136.168036,95.9665207 L136.168036,112.660562 L136.677736,112.660562 C144.102746,99.9650027 157.908637,92.3824528 172.605689,92.9280076 C211.050535,92.9280076 218.138927,118.216023 218.138927,151.114151 L218.123122,218.127392 Z M56.9550587,79.2685282 C44.7981969,79.2707099 34.9413443,69.4171797 34.9391618,57.260052 C34.93698,45.1029244 44.7902948,35.2458562 56.9471566,35.2436736 C69.1040185,35.2414916 78.9608713,45.0950217 78.963054,57.2521493 C78.9641017,63.090208 76.6459976,68.6895714 72.5186979,72.8184433 C68.3913982,76.9473153 62.7929898,79.26748 56.9550587,79.2685282 M75.9206558,218.127392 L37.94995,218.127392 L37.94995,95.9665207 L75.9206558,95.9665207 L75.9206558,218.127392 Z M237.033403,0.0182577091 L18.8895249,0.0182577091 C8.57959469,-0.0980923971 0.124827038,8.16056231 -0.001,18.4706066 L-0.001,237.524091 C0.120519052,247.839103 8.57460631,256.105934 18.8895249,255.9977 L237.033403,255.9977 C247.368728,256.125818 255.855922,247.859464 255.999,237.524091 L255.999,18.4548016 C255.851624,8.12438979 247.363742,-0.133792868 237.033403,0.000790807055" />
            </svg>
        </a>
    </div>

    <!-- Mobile hamburger -->
    <button
        class="lg:hidden p-2 text-slate-400 hover:text-white border border-white/10 rounded-lg hover:border-white/20 transition-all duration-200"
        type="button"
        on:click={toggleNav}
        aria-label="Toggle navigation">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/>
        </svg>
    </button>
</nav>

<!-- Mobile dropdown -->
<div
    class="small-nav fixed top-[65px] left-0 right-0 z-40 bg-[#0a0a0a]/95 backdrop-blur-md border-b border-white/5 lg:hidden"
    id="smallNav">
    <div class="px-6 py-6 flex flex-col gap-1">
        <a href="{base}/Projects" class="text-slate-300 hover:text-white transition-colors py-2 text-sm">Projects</a>
        <a href="{base}/Socials" class="text-slate-300 hover:text-white transition-colors py-2 text-sm">Socials</a>
        <div class="pt-3 mt-1 border-t border-white/10 flex gap-4">
            <a href="https://www.github.com/JulianJankowski" class="text-slate-400 hover:text-white transition-colors py-2 text-sm">GitHub</a>
            <a href="https://www.linkedin.com/in/julian-jankowski-b1636b151/" class="text-slate-400 hover:text-white transition-colors py-2 text-sm">LinkedIn</a>
        </div>
    </div>
</div>

{#key data.pathname}
    <div in:fade={{ duration: 200, delay: 200 }} out:fade={{ duration: 200 }} class="pt-[65px]">
        <slot />
    </div>
{/key}
