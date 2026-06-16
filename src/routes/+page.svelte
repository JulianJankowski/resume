<script>
    function sendEmail() {
        const body = /** @type {HTMLTextAreaElement|null} */ (document.getElementById('body'))?.value || '';
        window.location.href = `mailto:julian.jankowski@gmail.com?subject=Message from Resume Site&body=${encodeURIComponent(body)}`;
    }
</script>

<main>
    <!-- ── Hero ── -->
    <section class="relative min-h-screen flex items-center justify-center overflow-hidden px-6">
        <!-- Background: dot grid + glow orbs -->
        <div class="absolute inset-0 pointer-events-none">
            <div class="absolute inset-0 opacity-[0.12]"
                 style="background-image: radial-gradient(circle, #14b8a6 1px, transparent 1px); background-size: 32px 32px;">
            </div>
            <div class="absolute top-1/4 left-1/3 w-[600px] h-[600px] bg-teal-600/10 rounded-full blur-[140px]"></div>
            <div class="absolute bottom-1/4 right-1/4 w-[400px] h-[400px] bg-violet-600/10 rounded-full blur-[120px]"></div>
        </div>

        <div class="relative z-10 text-center max-w-5xl mx-auto">
            <!-- Name -->
            <h1 class="anim-fade-up anim-delay-1 text-5xl sm:text-7xl lg:text-8xl mb-6 bg-gradient-to-br from-white via-slate-100 to-slate-400 bg-clip-text text-transparent">
                Julian Jankowski
            </h1>

            <!-- Subtitle -->
            <p class="anim-fade-up anim-delay-2 text-lg sm:text-xl text-slate-400 mb-12 tracking-wide">
                Software Developer <span class="text-teal-500 font-semibold">·</span> Salesforce Consultant
            </p>

            <!-- CTAs -->
            <div class="anim-fade-up anim-delay-3 flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#work"
                   class="px-8 py-3.5 bg-teal-500 hover:bg-teal-400 text-black font-semibold rounded-xl transition-all duration-200 hover:shadow-lg hover:shadow-teal-500/20 hover:-translate-y-0.5">
                    View My Work
                </a>
                <a href="#contact"
                   class="px-8 py-3.5 bg-transparent border border-white/15 hover:border-teal-500/50 hover:bg-teal-500/5 text-white rounded-xl transition-all duration-200 hover:-translate-y-0.5">
                    Get in Touch
                </a>
            </div>
        </div>

        <!-- Scroll indicator -->
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2 text-slate-600">
            <span class="text-xs tracking-[0.2em] uppercase">Scroll</span>
            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 animate-bounce" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
            </svg>
        </div>
    </section>

    <!-- ── What I Bring ── -->
    <section id="work" class="py-28 px-6 scroll-mt-16">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-20">
                <p class="text-teal-400 text-xs font-semibold tracking-[0.2em] uppercase mb-3">About Me</p>
                <h2 class="text-3xl sm:text-4xl text-white mb-4">What I Bring</h2>
                <p class="text-slate-400 max-w-md mx-auto text-sm">A blend of technical depth, collaborative mindset, and genuine curiosity.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Developer -->
                <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-teal-500/40 hover:bg-teal-500/[0.04] transition-all duration-300 hover:-translate-y-1">
                    <div class="w-12 h-12 rounded-xl bg-teal-500/10 border border-teal-500/20 flex items-center justify-center mb-6 group-hover:bg-teal-500/20 transition-colors">
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 text-teal-400" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 6.75 22.5 12l-5.25 5.25m-10.5 0L1.5 12l5.25-5.25m7.5-3-4.5 16.5" />
                        </svg>
                    </div>
                    <h3 class="text-xl text-white mb-3">Developer</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Full Stack Developer comfortable across the entire stack — from backend services to polished UIs.
                        Agile team collaborator and independent worker.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        {#each ['Python', 'TypeScript', 'JavaScript', 'Java'] as tech}
                            <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300 font-mono">{tech}</span>
                        {/each}
                    </div>
                </div>

                <!-- Collaborator -->
                <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-violet-500/40 hover:bg-violet-500/[0.04] transition-all duration-300 hover:-translate-y-1">
                    <div class="w-12 h-12 rounded-xl bg-violet-500/10 border border-violet-500/20 flex items-center justify-center mb-6 group-hover:bg-violet-500/20 transition-colors">
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 text-violet-400" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.5">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M15 19.128a9.38 9.38 0 0 0 2.625.372 9.337 9.337 0 0 0 4.121-.952 4.125 4.125 0 0 0-7.533-2.493M15 19.128v-.003c0-1.113-.285-2.16-.786-3.07M15 19.128v.106A12.318 12.318 0 0 1 8.624 21c-2.331 0-4.512-.645-6.374-1.766l-.001-.109a6.375 6.375 0 0 1 11.964-3.07M12 6.375a3.375 3.375 0 1 1-6.75 0 3.375 3.375 0 0 1 6.75 0Zm8.25 2.25a2.625 2.625 0 1 1-5.25 0 2.625 2.625 0 0 1 5.25 0Z" />
                        </svg>
                    </div>
                    <h3 class="text-xl text-white mb-3">Collaborator</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Strong communicator with deep experience in agile environments and building out modern DevOps pipelines.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        {#each ['Git', 'Jira', 'Confluence', 'GitHub Actions', 'Bitbucket'] as tech}
                            <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300 font-mono">{tech}</span>
                        {/each}
                    </div>
                </div>

                <!-- Hobbyist -->
                <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-rose-500/40 hover:bg-rose-500/[0.04] transition-all duration-300 hover:-translate-y-1">
                    <div class="w-12 h-12 rounded-xl bg-rose-500/10 border border-rose-500/20 flex items-center justify-center mb-6 group-hover:bg-rose-500/20 transition-colors">
                        <!-- viewBox matches the Inkscape coordinate space; white background path removed; fills inherit currentColor -->
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 text-rose-400" viewBox="0 0 544 544" fill="currentColor" fill-rule="nonzero">
                            <g transform="translate(-35.14898,-25.367676)">
                                <path d="m 307.88531,378.24075 c -4.81658,1.77753 -10.2066,2.80966 -15.71127,2.80966 -5.90607,0 -11.75479,-0.68808 -17.1448,-2.23626 L 214.1337,518.78217 c -5.56201,12.90161 -20.87192,17.25946 -34.23224,9.74786 -13.30298,-7.5116 -19.61043,-23.96832 -13.87639,-36.8699 l 74.65726,-171.21854 95.18513,0 0,-15.99799 48.16596,-22.42013 c 12.6149,-6.13541 29.01425,4.35788 32.34002,17.7182 l 23.62424,94.72641 c 3.38309,13.41766 -4.81659,27.00735 -18.23425,30.3331 -13.47501,3.38309 -27.12204,-4.81659 -30.44776,-18.23425 l -15.02322,-60.37949 -68.40714,32.05331 z"/>
                                <path d="M 351.75076,280.13126 C 456.05301,228.41017 496.47803,51.228218 496.47803,36.434379 l -14.33512,0 C 476.7529,73.361633 431.97003,221.24261 351.75076,264.13327 l 0,15.99799 z"/>
                                <path d="m 159.31624,241.36911 c 5.44734,8.54373 16.45671,12.32819 26.20457,8.31436 l 55.16152,-21.61734 0,76.49216 95.18513,0 0,-88.59099 85.32257,-136.527587 c 6.25009,-9.977234 3.38309,-23.165535 -6.70883,-29.587662 -9.97723,-6.250111 -23.16553,-3.325737 -28.78491,6.422127 l -72.4783,115.999702 -43.63608,0.11469 c -2.80969,0 -5.61936,0.45872 -8.42905,1.5482 l -75.40268,29.58764 -38.87681,-58.88862 c -6.3648,-9.86255 -19.61043,-12.78691 -29.58767,-6.42214 -9.97723,6.42214 -12.84426,19.72512 -6.47947,29.70237 l 48.51001,73.45309 z"/>
                                <path d="m 281.73807,164.53293 c 20.9866,0 38.01672,-16.91544 38.01672,-37.8447 0,-20.92925 -17.03012,-37.959364 -38.01672,-37.959364 -20.92926,0 -37.95935,17.030114 -37.95935,37.959364 0,20.92926 17.03009,37.8447 37.95935,37.8447"/>
                                <path d="m 335.86746,551.81024 0,-170.75982 -15.99798,7.45425 0,163.30557 15.99798,0 z"/>
                            </g>
                        </svg>
                    </div>
                    <h3 class="text-xl text-white mb-3">Boulderer</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Passionate about bouldering — constantly working problems, improving technique, and exploring new crags.
                    </p>
                    <div class="flex flex-wrap gap-2">
                        {#each ['Bouldering', 'Problem Solving', 'Strength Training'] as tag}
                            <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300">{tag}</span>
                        {/each}
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ── Contact ── -->
    <section id="contact" class="py-28 px-6 scroll-mt-16">
        <!-- Subtle divider glow -->
        <div class="max-w-xl mx-auto">
            <div class="text-center mb-12">
                <p class="text-teal-400 text-xs font-semibold tracking-[0.2em] uppercase mb-3">Contact</p>
                <h2 class="text-3xl sm:text-4xl text-white mb-4">Get in Touch</h2>
                <p class="text-slate-400 text-sm">Have a project in mind or just want to say hi? Drop me a message.</p>
            </div>

            <div class="p-8 rounded-2xl bg-white/[0.03] border border-white/10">
                <form>
                    <div class="mb-5">
                        <label for="email" class="block text-xs text-slate-400 uppercase tracking-widest mb-2">Your Email</label>
                        <input
                            type="email"
                            name="email"
                            id="email"
                            autocomplete="email"
                            placeholder="you@example.com"
                            class="w-full px-4 py-3 bg-white/5 border border-white/10 rounded-xl text-white placeholder-slate-600 focus:outline-none focus:border-teal-500/50 focus:bg-teal-500/[0.03] transition-all duration-200 text-sm">
                    </div>
                    <div class="mb-6">
                        <label for="body" class="block text-xs text-slate-400 uppercase tracking-widest mb-2">Message</label>
                        <textarea
                            name="body"
                            id="body"
                            rows="5"
                            placeholder="Tell me about your project..."
                            class="w-full px-4 py-3 bg-white/5 border border-white/10 rounded-xl text-white placeholder-slate-600 focus:outline-none focus:border-teal-500/50 focus:bg-teal-500/[0.03] transition-all duration-200 text-sm resize-none"></textarea>
                    </div>
                    <button
                        type="button"
                        on:click={sendEmail}
                        class="w-full py-3.5 bg-teal-500 hover:bg-teal-400 text-black font-semibold rounded-xl transition-all duration-200 hover:shadow-lg hover:shadow-teal-500/20">
                        Send Message
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- ── Footer ── -->
    <footer class="py-8 px-6 border-t border-white/5">
        <div class="max-w-6xl mx-auto flex flex-col sm:flex-row items-center justify-between gap-4">
            <p class="text-slate-600 text-sm">© 2025 Julian Jankowski</p>
            <div class="flex gap-6">
                <a href="https://github.com/JulianJankowski" class="text-slate-500 hover:text-white text-sm transition-colors duration-200">GitHub</a>
                <a href="https://www.linkedin.com/in/julian-jankowski-b1636b151/" class="text-slate-500 hover:text-white text-sm transition-colors duration-200">LinkedIn</a>
            </div>
        </div>
    </footer>
</main>
