<script>
	let mobileOpen = $state(false);

	const links = [
		{ label: 'Research Questions', href: '#research-questions' },
		{ label: 'Hypothesis', href: '#hypothesis' },
		{ label: 'Objectives', href: '#objectives' },
		{ label: 'Data', href: '#data' },
		{ label: 'Results', href: '#results' },
		{ label: 'About', href: '#about' }
	];

	function handleClick() {
		mobileOpen = false;
	}
</script>

<nav class="sticky inset-x-0 top-0 z-50 border-b border-border bg-surface/80 backdrop-blur-md">
	<div class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4">
		<a
			href="https://mcjefdreal.github.io/michair-jurban/"
			class="text-lg font-bold tracking-tight text-text-primary transition-colors hover:text-accent"
		>
			michAIR jURBAN
		</a>

		<!-- Desktop links -->
		<div class="hidden items-center gap-8 md:flex">
			{#each links as link}
				<a
					href={link.href}
					class="group relative text-sm font-medium text-text-secondary transition-colors hover:text-accent"
				>
					{link.label}
					<span
						class="absolute -bottom-1 left-0 h-0.5 w-0 bg-accent transition-all duration-300 group-hover:w-full"
					></span>
				</a>
			{/each}
		</div>

		<!-- Mobile hamburger -->
		<button
			class="rounded-lg p-2 transition-colors hover:bg-surface-alt md:hidden"
			onclick={() => (mobileOpen = !mobileOpen)}
			aria-label="Toggle menu"
		>
			<svg class="h-6 w-6 text-text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
				{#if mobileOpen}
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M6 18L18 6M6 6l12 12"
					/>
				{:else}
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h16M4 18h16"
					/>
				{/if}
			</svg>
		</button>
	</div>

	<!-- Mobile menu -->
	{#if mobileOpen}
		<div class="border-t border-border bg-surface/95 backdrop-blur-md md:hidden">
			<div class="flex flex-col gap-3 px-6 py-4">
				{#each links as link}
					<a
						href={link.href}
						class="py-2 text-sm font-medium text-text-secondary transition-colors hover:text-accent"
						onclick={handleClick}
					>
						{link.label}
					</a>
				{/each}
			</div>
		</div>
	{/if}
</nav>
