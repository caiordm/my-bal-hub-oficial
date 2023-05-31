<script>
	import CardHistory from '../../components/CardHistory.svelte';
	import mais from '../../images/mais.png';

	function handler() {
		alert("Calma irmões");
	}
</script>

<main>
	<div class="header">
		<span>
			<h1>Olá NOME!</h1>
			<h4>Uma nova história?</h4></span
		>
		<button on:click={handler}>New History <img src={mais} alt="Adicionar" /></button>
	</div>
	<div class="content">
		<CardHistory
			colorBg2="#386153"
			avatar="https://cdn-icons-png.flaticon.com/512/147/147144.png"
			nomeProtagonista="Konno Soumaré"
			nacionalidade="Costa do Marfim"
			timeAtual="Hebei"
			dataInicio="01/02/2020"
		/>
		<CardHistory
			colorBg2="#3065ac"
			avatar="https://cdn-icons-png.flaticon.com/512/147/147144.png"
			nomeProtagonista="Josue Louccura"
			nacionalidade="Portugal"
			timeAtual="Monaco"
			dataInicio="04/11/2022"
		/>
		<CardHistory
			colorBg2="#1120c3"
			avatar="https://cdn-icons-png.flaticon.com/512/147/147144.png"
			nomeProtagonista="Hendrux Caladge"
			nacionalidade="Países Baixos"
			timeAtual="AZ ALkmaar"
			dataInicio="12/12/2021"
		/>
	</div>
</main>

<style>
	:root {
		--light-green: #00ffea;
		--mid-green: #00b1a3;
		--black: #000000;
		--white: #ffffff;
		--main-blue: #0035bb;
		--light-gray: #dadada;
		--gray: #cbcbcb;
		--dark-gray: #a3a3a3;
	}

	main {
		font-family: 'Big Shoulders Display', cursive;
		min-width: 80vw;
		min-height: 80vh;
		display: flex;
		flex-direction: column;
	}

	.header {
		max-width: 90rem;
		border-bottom: 1px solid #cccccc;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0rem 3rem;
	}

	.content {
		display: flex;
		flex-direction: column;
		gap: 2rem;
		padding: 1rem 3rem;
	}

	span {
		display: flex;
		justify-content: center;
		align-items: baseline;
		gap: 0.4rem;
	}

	h1 {
		font-size: 26pt;
	}

	h4 {
		font-size: 22pt;
	}

	button {
		width: 12rem;
		height: 4rem;
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 0.6rem;

		background-color: var(--main-blue);
		border-radius: 10px;
		border: none;
		
		color: var(--white);
		font-family: 'Big Shoulders Display', cursive;
		font-weight: 700;
		font-size: 18pt;

		cursor: pointer;
	}
</style>
