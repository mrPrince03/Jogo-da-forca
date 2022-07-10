<svelte:head>
	<link rel="stylesheet" href="/styles/menu.css">
</svelte:head>

<script>
	import { estado } from './Estado.js'
	import { trocarEstadoDoJogo } from './Estado.js'
</script>

<h1>
	Jogo da Forca
</h1>

<div class='menu' on:click={() => trocarEstadoDoJogo('jogar')}>
	Jogar
</div>

<div class='menu' on:click={() => trocarEstadoDoJogo('regras')}>
	Regras
</div>

<div class='menu' on:click={() => trocarEstadoDoJogo('sobre')}>
	Sobre
</div>

