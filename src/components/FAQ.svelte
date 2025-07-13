<script>
	import Accordion from './common/Accordion.svelte';
	const items = [
		{
			q: 'Adakah IQ Option sah di Malaysia?',
			a: 'Walaupun tidak dikawal selia oleh pihak berkuasa Malaysia, IQ Option boleh diakses dan digunakan secara meluas oleh pedagang di Malaysia.'
		},
		{
			q: 'Adakah IQ Option satu penipuan?',
			a: 'Tidak, IQ Option ialah platform yang sah yang dipercayai oleh berjuta-juta pengguna di seluruh dunia dan disokong oleh operasi yang terbukti selama bertahun-tahun.'
		},
		{
			q: 'Bolehkah IQ Option dipercayai?',
			a: 'Ya, platform ini mempunyai reputasi yang kukuh dan menggunakan amalan selamat seperti penyulitan SSL dan pengesahan dua faktor.'
		},
		{
			q: 'Adakah IQ Option percuma untuk digunakan?',
			a: 'Ya, tiada caj dikenakan untuk pendaftaran akaun atau deposit.'
		},
		{
			q: 'Adakah IQ Option dan IQ Broker adalah syarikat yang sama?',
			a: 'Ya, ia adalah jenama yang berbeza di bawah organisasi induk yang sama.'
		}
	];
</script>

<section>
	<h2>Soalan Lazim</h2>

	{#each items as item, idx}
		{#if idx === 0}
			<Accordion open {item} />{:else}<Accordion {item} />{/if}
	{/each}
</section>

<style>
	h2 {
		margin-bottom: 10px;
	}
	h3 {
		text-align: center;
		margin-bottom: 40px;
		margin-top: 0;
	}
</style>
