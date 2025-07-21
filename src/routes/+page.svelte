<script>
	import { base } from '$app/paths';
	import meta__img from '$lib/images/meta__img.jpg';
	import AllBlocks from '../components/AllBlocks.svelte';

	const title = 'IQ Option - Apa itu, Bagaimana Daftar, Log Masuk, Dagangan di Malaysia';
	const desc =
		'IQ Option: Ketahui apa itu, cara daftar dan log masuk di Malaysia. Mudah untuk pemula dan pedagang berpengalaman.';
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
