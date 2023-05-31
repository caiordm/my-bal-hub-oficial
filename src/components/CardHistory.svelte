<script>
	import '../global.css';

	export let colorBg2 = '';
	export let avatar = '';
	export let nomeProtagonista = '';
	export let nacionalidade = '';
	export let timeAtual = '';
	export let dataInicio = '';
</script>

<a href="www.santacruzpe.com.br" id="card">
	<div class="bg2" style="background-color: {colorBg2};">
		<img src={avatar} alt="History Avatar" />
	</div>
	<div class="texts">
		<p id="nameTitle" style="text-decoration: underline {colorBg2};">{nomeProtagonista}</p>
		<p>Nacionalidade: {nacionalidade}</p>
		<p>Clube Atual: {timeAtual}</p>
		<p>Inicio da Carreira: {dataInicio}</p>
	</div>
</a>

<style>
	#card {
		text-decoration: none;
		height: 10rem;
		width: 60rem;
		display: flex;
		font-family: 'Big Shoulders Display', cursive;
		gap: 1rem;

		background-color: #f0ebeb;
		border: 1px solid #cccccc;
		border-radius: 10px;
	}

	.bg2 {
		width: 10rem;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		border-radius: 10px 0px 0px 10px;
	}

	img {
		max-width: 7rem;
	}

	.texts {
		display: flex;
		flex-direction: column;
		color: #252627;
		padding: 0.4rem;
	}

	p {
		display: flex;
		margin: 0;
		font-size: 18pt;
		font-weight: 600;
	}

	#nameTitle {
		font-weight: 700;
		font-size: 26pt;
		margin-bottom: 1rem;
	}
</style>
