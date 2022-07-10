<svelte:head>
	<link rel="stylesheet" href="/styles/jogar.css">
</svelte:head>

<script>
	import VoltarMenu from './VoltarMenu.svelte'
	import { estado } from "./Estado.js"
	import { trocarEstadoDoJogo } from './Estado.js'
	import Button from './Button.svelte'
////--------------SORTEIO DA PALAVRA--------------\\\\

let palavras = [
		["cama", "objeto"],
		["aviao", "transporte"],
		["mouse", "objeto"]
]

function sorteioPalavra(palavras) {
	const aux =  Math.floor(Math.random() * palavras.length)
    return palavras[aux]
}

console.log(sorteioPalavra(palavras));

////--------------SORTEIO DA PALAVRA--------------\\\\


	</script>


<p>

<div id='dicas'>
</div>

	<p>
	
	</p>


		<div id="imgforca">

		</div>

			<div id="palavra-misteriosa">
				<div class="letras">A</div>
				<div class="letras">V</div>
				<div class="letras">I</div>
				<div class="letras">A</div>
				<div class="letras">O</div>
				</div>
					<br>
					<br>
					<br>
					<div id="teclas">
						<div class="botao">	
							<Button on:click={'A'}>A</Button>
							<Button on:click={'B'}>B</Button>
							<Button on:click={'C'}>C</Button>
							<Button on:click={'D'}>D</Button>
							<Button on:click={'E'}>E</Button>
							<Button on:click={'F'}>F</Button>
							<Button on:click={'G'}>G</Button>
							<Button on:click={'H'}>H</Button>
							<Button on:click={'I'}>I</Button>
							<Button on:click={'J'}>J</Button>
							<Button on:click={'K'}>K</Button>
							<Button on:click={'L'}>L</Button>
							<Button on:click={'M'}>M</Button>
					</div>
					<div class="botao">
						<Button on:click={'N'}>N</Button>
						<Button on:click={'O'}>O</Button>
						<Button on:click={'P'}>P</Button>
						<Button on:click={'Q'}>Q</Button>
						<Button on:click={'R'}>R</Button>
						<Button on:click={'S'}>S</Button>
						<Button on:click={'T'}>T</Button>
						<Button on:click={'U'}>U</Button>
						<Button on:click={'W'}>W</Button>
						<Button on:click={'X'}>X</Button>
						<Button on:click={'Y'}>Y</Button>
						<Button on:click={'Z'}>Z</Button>
					</div>
				</div>
				
					








						<VoltarMenu/>