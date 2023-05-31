<script>
    import "../../global.css";
</script>

<main>
    <div class="forms">
        <form action="/home">
            <h3>ENTRAR</h3>
            <div class="inputs">
                <input type="email" name="email" placeholder="Seu e-mail" required>
                <input type="password" name="password" placeholder="Sua senha" required>
            </div>
            <button type="submit">Entrar</button>
            <a href="/signup">Não tem conta? Cadastre-se</a>
        </form>
    </div>
    <div class="contents">
        <div class="texts">
            <h2>My</h2>
            <h2 class="text-green">BECOME A LEGEND</h2>
            <h2>Hub</h2>
            <h4>Documente sua história e seus feitos no Rumo ao Estrelato, desde títulos, recordes, clubes, estatísticas e muito mais.</h4>
        </div>
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
    min-height: 100vh;
    display: flex;
}

.contents {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 50%;
    background-image: linear-gradient(to right bottom, #0038d8, #0035bb, #00319d, #002b80, #002563);
    color: var(--white);
}

h2 {
    font-size: 28pt;
}

.text-green {
    color: var(--light-green);
}

.contents h4 {
    max-width: 400px;
    font-size: 18pt;
    margin-top: 2em;
    margin-bottom: 2rem;

}

.forms {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 50%;
    background-image: url('https://wallpapercave.com/wp/wp9511127.jpg');
    background-size: cover;
}


form {
    padding: 1rem;
    width: 22rem;
    height: 30rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;
    background: rgba(255, 255, 255, 0.25);
    box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(18px);
    -webkit-backdrop-filter: blur(18px);
    border-radius: 10px;
    border: 1px solid rgba(255, 255, 255, 0.18);
}

form h3 {
    margin-top: 1rem;
    font-size: 20pt;
    color: var(--white);
}

.inputs {
    margin-top: 2rem;
    display: flex;
    flex-direction: column;
    gap: 0.6em;
}

input {
    padding: 0.6rem;
    border-radius: 4px;
    border: 1px solid #8d8d8d9b;
    font-size: 12pt;
    font-family: 'Open Sans', sans-serif;
}

button {
    background-color: var(--white);
    border: none;
    border-radius: 20px;
    font-size: 16pt;
    font-weight: 600;
    padding: 0.4rem;
    transition: 0.25s ease-in-out;
}

a {
    color: var(--white);
    font-size: 16pt;
    text-decoration: none;
    font-weight: 600;
    width: 12.5rem;
    border-bottom: 2px solid var(--white);
    transition: 0.25s ease-in-out;
}

a:hover {
    border-bottom: 2px solid var(--black);
    color: var(--black);

}

input:focus {
    outline: solid 1px var(--black);
}

button:hover {
    border-radius: 4px;
    background-color: var(--black);
    color: var(--white);
    cursor: pointer;
}
</style>