<script lang="ts">
	// HTTP response data provided by +page.ts
	import type { PageData } from './$types';
	export let data: PageData;
	$: ({ contributors } = data);
</script>

<div>
	<!-- Promo Banner -->
	<div class="variant-filled-primary p-4">
		<div class="w-full max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-[1fr_auto] gap-4">
			<div class="flex items-center gap-6">
				<span class="text-xl">🎉</span>
				<p class="text-lg">The Skeleton v3 Beta is now available!</p>
			</div>
			<div class="flex gap-4">
				<a class="btn variant-filled" href="https://github.com/skeletonlabs/skeleton/discussions/2919" target="_blank">Learn More</a>
				<a class="btn variant-filled" href="https://github.com/skeletonlabs/skeleton/discussions/2921" target="_blank">Migration Guide</a>
			</div>
		</div>
	</div>
</div>

<style lang="postcss">
	.section-container {
		@apply w-full max-w-7xl mx-auto p-4 py-16 md:py-24;
	}
	/* Hero Gradient */
	/* prettier-ignore */
	.hero-gradient {
		background-image:
			radial-gradient(at 0% 0%, rgba(var(--color-secondary-500) / 0.33) 0px, transparent 50%),
			radial-gradient(at 98% 1%, rgba(var(--color-error-500) / 0.33) 0px, transparent 50%);
	}
	/* SvelteKit Gradient */
	/* prettier-ignore */
	.sveltekit-gradient {
		background-image:
			radial-gradient(at 0% 100%, rgba(var(--color-secondary-500) / 0.50) 0px, transparent 50%);
	}
	/* SvelteKit Gradient */
	/* prettier-ignore */
	.tailwind-gradient {
		background-image:
			radial-gradient(at 0% 0%, rgba(var(--color-secondary-500) / 0.50) 0px, transparent 50%),
			radial-gradient(at 100% 100%,  rgba(var(--color-primary-500) / 0.24) 0px, transparent 50%);
	}
	/* Features Gradient */
	/* prettier-ignore */
	.features-gradient {
		background-image:
			radial-gradient(at 0% 0%, rgba(var(--color-secondary-500) / 0.33) 0px, transparent 50%),
			radial-gradient(at 100% 0%,  rgba(var(--color-primary-500) / 0.33) 0px, transparent 50%);
	}
	/* Sponsors Gradient */
	/* prettier-ignore */
	.sponsors-gradient {
		background-image:
		radial-gradient(at 0% 99%, rgba(var(--color-error-500) / 0.23) 0px, transparent 50%),
		radial-gradient(at 100% 100%, rgba(var(--color-primary-500) / 0.19) 0px, transparent 50%);
	}
	/* Radial */
	/* prettier-ignore */
	.bottom-cta-gradient {
		@apply bg-primary-500 text-on-primary-token;
		background-image:
		radial-gradient(at 0% 0%, rgba(var(--color-secondary-500) / 0.75) 0px, transparent 40%),
		radial-gradient(at 100% 100%, rgba(var(--color-secondary-500) / 0.75) 0px, transparent 40%);
	}
</style>
