<script>
	import { base } from '$app/paths';
</script>

<div class="bgr" style="color: #fff; position: relative;">
	<div
		class="bgr-gradient"
		style="height: 100%; left: 0; position: absolute; top: 0; width: 100%; background: #000; background: linear-gradient(180deg, rgba(122, 0, 147, 0.85), rgba(3, 6, 126, 0.85)); z-index: 0;"
	></div>
	<div
		class="bgr-img"
		style="background-position: 50%; background-repeat: repeat; background-size: cover; height: 100%; left: 0; position: absolute; top: 0; width: 100%; will-change: transform; z-index: -1; background-image: url({base}/images/bg_intro.webp);"
	></div>
	<section style="position: relative; z-index: 2;">
		<div class="intro" style="margin: 0 auto; text-align: center; padding: 140px 0 100px;">
			<h1>
				<span>IQ Option Malaysia</span>
				<span>Platform Overview, Features, and Pros & Cons</span>
			</h1>
			<!-- <p style="font-size: 18px;">
				Hoje, negociar é uma das opções para ganhar dinheiro extra sem grandes investimentos.
				Escolher uma corretora confiável e uma plataforma simples e fácil de entender pode ser
				crucial, principalmente para iniciantes. Neste artigo você aprenderá <b
					>como usar IQ Option</b
				> e como ganhar dinheiro.
			</p> -->
		</div>
	</section>
</div>

<style>
	h1 span:first-child {
		position: relative;
		padding-bottom: 16px;
		margin-bottom: 16px;
	}

	h1 span {
		display: block;
	}

	h1 span:first-child:after {
		content: '';
		position: absolute;
		width: 100px;
		height: 1px;
		background-color: rgba(255, 255, 255, 0.4);
		left: calc(50% - 50px);
		bottom: 0;
	}
</style>
