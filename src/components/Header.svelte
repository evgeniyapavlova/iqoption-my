<script>
	import { onMount, onDestroy } from 'svelte';
	import LogoIQOption from './common/LogoIQOption.svelte';

	let scrolled = false;

	const handleScroll = () => {
		scrolled = window.scrollY > 0;
	};

	onMount(() => {
		if (typeof window !== 'undefined') {
			window.addEventListener('scroll', handleScroll);
		}
	});

	onDestroy(() => {
		if (typeof window !== 'undefined') {
			window.removeEventListener('scroll', handleScroll);
		}
	});
</script>

<header class:scrolled>
	<section>
		<LogoIQOption />

		<a href="#registration" class="button">Sign up</a>
	</section>
</header>

<style>
	/* .letters {
		fill: #fff;
		transition: fill 300ms linear;
	} */
	header.scrolled {
		background-color: white;
		box-shadow: rgba(0, 0, 0, 0.05) 0px 0px 16px 1px;
		--Logo-Primary: #000;
	}

	/* header.scrolled .letters {
		fill: #000;
	} */

	header {
		transition: background-color 300ms linear;
		padding: 16px 0;
		position: fixed;
		z-index: 3;
		width: 100%;

		--Logo-Primary: #fff;
	}
	/* svg {
		display: block;
	} */

	section {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	@media screen and (max-width: 960px) {
		header {
			padding: 14px 0;
		}
		:global(header .button) {
			padding: 10px 22px 11px;
			font-size: 12px;
		}
	}
</style>
