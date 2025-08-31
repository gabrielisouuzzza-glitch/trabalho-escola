se tudo der erradp:

index : <!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <title>Tropicália</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-icons/1.11.3/font/bootstrap-icons.min.css">
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header class=" p-5">

        <nav class="container d-flex justify-content-between align-items-center">
            <img src="imagens/logo.oidr2.png" alt="Logotipo" class="nav-img " loading="lazy">
            <ul class="nav mt-5">
                <li class="nav-item"><a class="nav-link" href="#inicio">Início</a></li>
                <li class="nav-item"><a class="nav-link" href="#galeria">Galeria</a></li>
                <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>
            </ul>          
        </nav>
       
    </header>


    <main class="container my-5">

        <section id="inicio" class="my-5">
            <div class="inicio-fundo d-flex justify-content-between align-items-center">
                <div class="esquerda-conteudo">
                    <h1 class="display-5 text-white fw-bold">Conheça mais sobre:</h1>
                    <img src="imagens/cultura.png" alt="Logotipo secundário da Tropicália" class="mb-3" width="563"
                        height="300" loading="lazy">
                    <a href="#tropicalia"
                        class="btn btn-primary btn-lg botao-inicio fw-semibold">Quero
                        conhecer!</a>
                </div>

            </div>
        </section>

        <section id="tropicalia" class="my-5 pt-6 secao-tropicalia">
            <div class="container d-flex align-items-center ">
                  <div class="col-5">
                    <h2>Como foi o início?</h2>
                    <p class="p-2">O rock no Brasil começou a ganhar destaque na década de 1950,
                        influenciado pelo rock and roll americano. A gravação de "Rock Around the Clock"
                        por Nora Ney em 1955 é frequentemente citada como o marco inicial, embora a música
                        original fosse de Bill Haley & His Comets. Nos anos seguintes, artistas como Cauby
                        Peixoto, Roberto Carlos e Erasmo Carlos começaram a explorar o gênero, 
                        adaptando-o ao contexto brasileiro. A Jovem Guarda, nos anos 60, foi um movimento
                        importante na popularização do rock, com artistas como Roberto Carlos, Erasmo Carlos e Wanderléia. 
                </div>
            </div>
        </section>

        <section id="galeria">
            <h2 class="text-center pt-5">Galeria</h2>
            <div class="container p-3 mt-3 fundo-galeria ">

                <div class="row justify-content-md-center">
                    <div class="col-md-4">
                        <img src="imagens/chaene.png"
                            class="img-fluid rounded-5" loading="lazy">
                    </div>
                    <div class="col-md-4">
                        <img src="imagens/chuck.png" class="img-fluid rounded-5"
                            loading="lazy">
                    </div>
                </div>
            </div>
        </section>

        <section id="contato">
            <div class="container p-5 d-flex justify-content-center">
                <div class="col-md-8 col-lg-10 rounded-5 formulario"> <!-- Caixa do formulário com 60% de largura -->
                    <h2 class="mb-3">Entre em contato</h2>
                    <form>
                        <div class="form-group mb-3">
                            <label for="nome">Nome</label>
                            <input type="text" id="nome" name="nome" class="form-control rounded-3 mt-1"
                                placeholder="Digite seu nome completo">
                        </div>
                        <div class="form-group mb-3">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" class="form-control rounded-3 mt-1"
                                placeholder="Digite seu email">
                        </div>
                        <div class="form-group mb-3">
                            <label for="mensagem">Mensagem</label>
                            <textarea id="mensagem" name="mensagem" class="form-control rounded-4 mt-2" rows="4"
                                placeholder="Escreva sua mensagem"></textarea>
                        </div>
                        <div class="d-grid gap-2">
                            <button type="submit" class="btn btn-primary btn-lg rounded-pill tamanho-botao">Enviar
                                mensagem</button>
                        </div>
                    </form>
                </div>
            </div>
        </section>
    </main>
    <footer class="text-center p-3 fst-italic">
        <p>Acesse nossas redes:</p>
        <i class="bi bi-whatsapp"></i>
        <i class="bi bi-instagram"></i>
        <i class="bi bi-tiktok"></i>
        <p class="mt-3">Desenvolvido por Gabrieli Melzani de Souza.</p>
    </footer>
    <script src="script.js"></script>

</body>

</html>







style : @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lemon&display=swap');

:root {
    --laranja-claro: #818181;
}

body {
    font-size: 1rem;
    font-family: 'Montserrat';
}

header {
    background-color: #ffffff;
}


section {
    padding-bottom: 5rem;
}


.nav-link {
    color: #f391bf;
    font-weight: 600;
}

.inicio-fundo {
    /* aula 3 */
    background-image: url('imagens/fundinhorosa2.png');
    /* Substitua pelo caminho da sua imagem */
    background-size: cover;
    background-position: right;
    border-radius: 80px;
    width: 100%;
    height: 606px;
    padding: 40px;
    margin: 0 auto;
}

/* posicionamento para a imagem à direita */
.img-inicio {
    position: absolute;
    right: 0;
    top: 18rem;
    width: 45rem;
    height: auto;
}


.esquerda-conteudo {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 1rem;
}


.botao-inicio {
    background-color: var(--laranja-claro);
    border-radius: 30px;
    border: none;
    width: 14em;
    /* Convertido para em aumenta o tamanho da fonte por tabela*/
    height: 3em;
    /* Convertido para em */
    align-content: center;

}

.display-4 {
    text-shadow: -5px 5px var(--laranja-claro);
}


#tropicalia {
    position: relative;
    padding-top: 5rem;
    margin-top: 3rem;
    margin-bottom: 3rem;
    background: url('imagens/5\ Sem\ Título_20250819142007.png') top right no-repeat,
        url('imagens/6\ Sem\ Título_20250819142137.png') bottom left no-repeat;
    background-size:250px 250px;
    /* Ajuste o tamanho conforme necessário */
}

#tropicalia .container {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    z-index: 1;
    /* Garante que o conteúdo fica acima das imagens do background */
}


h2 {
    font-family: 'Lemon', serif;
    font-size: 2.5em;
    font-style: normal;
    color: var(--laranja-claro);
}

#galeria {
    background-color: #FAF4F4;

}

.fundo-galeria {
    background: url('imagens/zoios.png') bottom right no-repeat;
    background-size: 200px 200px;
}

#contato {
    background-image: url('imagens/fundinhorosa2.png');
    background-size: cover;
    padding: 4rem 0;
    /* Espaçamento interno para a seção de contato */

}

.formulario {
    background-color: #ffffff;
    padding: 2rem;
    /* Espaçamento interno dentro do formulário */
    border-radius: 10px;
    /* Borda arredondada para o formulário */
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    /* Sombra suave para destacar o formulário */
    font-weight: bold;
}

.formulario button {
    background-color: #c48db1;
    border: none;
    font-weight: bold;
}

/* chama classe do bootstrap para modificar a cor */
.form-control {
    background-color: #F1EDEF;
}


