<script>
    let mobileOpen = $state(false);

    const links = [
        { label: 'Research Questions', href: '#research-questions' },
        { label: 'Hypothesis', href: '#hypothesis' },
        { label: 'Objectives', href: '#objectives' },
        { label: 'Data', href: '#data' },
        { label: 'Results', href: '#results' },
        { label: 'About', href: '#about' },
    ];

    function handleClick() {
        mobileOpen = false;
    }
</script>

<nav class="sticky inset-x-0 top-0 z-50 bg-surface/80 backdrop-blur-md border-b border-border">
    <div class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
        <a href="/" class="text-lg font-bold text-text-primary tracking-tight hover:text-accent transition-colors">
            michAIR jURBAN
        </a>

        <!-- Desktop links -->
        <div class="hidden md:flex items-center gap-8">
            {#each links as link}
                <a
                    href={link.href}
                    class="text-sm font-medium text-text-secondary hover:text-accent transition-colors relative group"
                >
                    {link.label}
                    <span class="absolute -bottom-1 left-0 w-0 h-0.5 bg-accent group-hover:w-full transition-all duration-300"></span>
                </a>
            {/each}
        </div>

        <!-- Mobile hamburger -->
        <button
            class="md:hidden p-2 rounded-lg hover:bg-surface-alt transition-colors"
            onclick={() => mobileOpen = !mobileOpen}
            aria-label="Toggle menu"
        >
            <svg class="w-6 h-6 text-text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                {#if mobileOpen}
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                {:else}
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                {/if}
            </svg>
        </button>
    </div>

    <!-- Mobile menu -->
    {#if mobileOpen}
        <div class="md:hidden border-t border-border bg-surface/95 backdrop-blur-md">
            <div class="px-6 py-4 flex flex-col gap-3">
                {#each links as link}
                    <a
                        href={link.href}
                        class="text-sm font-medium text-text-secondary hover:text-accent transition-colors py-2"
                        onclick={handleClick}
                    >
                        {link.label}
                    </a>
                {/each}
            </div>
        </div>
    {/if}
</nav>
