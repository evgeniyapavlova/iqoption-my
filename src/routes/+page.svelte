<script>
	import { base } from '$app/paths';
	import meta__img from '$lib/images/meta__img.jpg';
	import AllBlocks from '../components/AllBlocks.svelte';

	const title = 'IQ Option Malaysia — Platform Overview, Features, and Pros & Cons';
	const desc =
		'IQ Option might already be on your radar if you live in Malaysia and want a feature-rich, easily available trading platform.';
</script>

<svelte:head>
	<title>{title}</title>
	<meta name="description" content={desc} />
	<meta property="og:title" content={title} />
	<meta property="og:description" content={desc} />
	<meta property="og:image" content={meta__img} />

	<meta name="twitter:site" content="iqoption.my" />
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content={title} />
	<meta name="twitter:description" content={desc} />
	<meta name="twitter:image" content={meta__img} />
	<link
		rel="preload"
		as="image"
		href="{base}/images/bg_intro.webp"
		type="image/webp"
		fetchpriority="high"
	/>
</svelte:head>

<AllBlocks />
