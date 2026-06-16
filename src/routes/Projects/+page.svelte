<main class="min-h-screen py-20 px-6">
    <div class="max-w-5xl mx-auto">

        <div class="mb-16">
            <p class="text-teal-400 text-xs font-semibold tracking-[0.2em] uppercase mb-3">Portfolio</p>
            <h2 class="text-3xl sm:text-4xl text-white mb-4">Projects</h2>
            <p class="text-slate-400 text-sm max-w-md">A selection of projects I've built.</p>
        </div>

        <div class="space-y-8">
            <!-- Project: Model Viewer -->
            <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-teal-500/30 transition-all duration-300">
                <div class="flex flex-col md:flex-row md:items-start gap-6">
                    <div class="flex-1">
                        <div class="flex items-center gap-3 mb-4">
                            <h3 class="text-xl text-white">Web Based Model Viewer</h3>
                            <a
                                href="https://github.com/JulianJankowski/model-viewer"
                                aria-label="GitHub repository"
                                class="p-1.5 text-slate-500 hover:text-white hover:bg-white/5 rounded-lg transition-all duration-200">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor">
                                    <path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" />
                                </svg>
                            </a>
                        </div>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6">
                            A web-based .STL file viewer for managing 3D models hosted on an external platform.
                            Features in-browser rendering, search and tag functionality, and direct downloading
                            without granting access to the host's file system.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            {#each ['3D Rendering', 'Web', 'File Management'] as tag}
                                <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300">{tag}</span>
                            {/each}
                        </div>
                    </div>
                </div>
            </div>

            <!-- Project: Obsidian Comments -->
            <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-amber-500/30 transition-all duration-300">
                <div class="flex flex-col md:flex-row md:items-start gap-6">
                    <div class="flex-1">
                        <div class="flex items-center gap-3 mb-4">
                            <h3 class="text-xl text-white">Obsidian Comments</h3>
                            <a
                                href="https://github.com/JulianJankowski/obsidian-comments"
                                aria-label="GitHub repository"
                                class="p-1.5 text-slate-500 hover:text-white hover:bg-white/5 rounded-lg transition-all duration-200">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor">
                                    <path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" />
                                </svg>
                            </a>
                        </div>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6">
                            An Obsidian plugin that brings Google Docs-style inline comments to your notes.
                            Select any text, write a comment, and it appears highlighted in the editor with a
                            sidebar panel for managing, resolving, and navigating all comments. Uses fuzzy
                            re-anchoring so comments survive edits elsewhere in the document.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            {#each ['TypeScript', 'Obsidian API', 'Plugin Dev'] as tag}
                                <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300 font-mono">{tag}</span>
                            {/each}
                        </div>
                    </div>
                </div>
            </div>

            <!-- Project: This Site -->
            <div class="group p-8 rounded-2xl bg-white/[0.03] border border-white/10 hover:border-violet-500/30 transition-all duration-300">
                <div class="flex flex-col md:flex-row md:items-start gap-6">
                    <div class="flex-1">
                        <div class="flex items-center gap-3 mb-4">
                            <h3 class="text-xl text-white">This Site</h3>
                            <a
                                href="https://github.com/JulianJankowski/resume"
                                aria-label="GitHub repository"
                                class="p-1.5 text-slate-500 hover:text-white hover:bg-white/5 rounded-lg transition-all duration-200">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4" viewBox="0 0 24 24" fill="currentColor">
                                    <path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" />
                                </svg>
                            </a>
                        </div>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6">
                            A personal resume and portfolio site built with SvelteKit and deployed to GitHub Pages.
                            Showcases projects, skills, and contact information with a clean dark aesthetic.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            {#each ['SvelteKit', 'Tailwind CSS', 'GitHub Pages'] as tag}
                                <span class="px-2.5 py-1 text-xs bg-white/5 border border-white/10 rounded-lg text-slate-300 font-mono">{tag}</span>
                            {/each}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</main>
