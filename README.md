<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portifolho</title>
    <style>
        /* 
  Variáveis para cores:
  --fundo-principal
  --texto
  --texto-inverso
  --destaque
  --destaque-inverso
  --fundo-card
*/

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root{
  --fundo-principal:#f5f5f5;
  --texto:#222222;
  --texto-inverso:#ffffff;
  --destaque:#0077ff;
  --destaque-inverso:#66bbff;
  --fundo-card:#ffffff;
}

body{
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  line-height: 1.5em;
  background-color: var(--fundo-principal);
  color: var(--texto);
}

header{
  background-color: var(--destaque);
  color: var(--texto);
  padding: 10px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

nav#menu ul{
  list-style: none;
  display: flex;
  gap: 10px;
}

nav#menu a {
  text-decoration: none;
  color: var(--texto-inverso);
  font-weight: 600;
  padding: 12px 15px;
  border-radius: 5px;
  transition: background-color 0.5s;
}
nav#menu a:hover{
  background-color: var(--destaque-inverso);
  color: var(--destaque);
}
main{
  display: grid;
  grid-template-columns: auto 90vw auto;
}

section#ficha{
  background-color: var(--fundo-card);
  padding: 20px;
  margin-bottom:15p ;
  border-radius: 8px;
  grid-column: 2;
}

section#ficha img.foto{
  width: 200px;
  aspect-ratio: 1/1;
  object-fit: cover;
  border-radius: 50%;
  border: 5px solid var(--fundo-card);
  outline:5px solid var(--destaque);
  display: block;
  margin: auto;
  margin-bottom: 15px;
}

section#ficha h1{
  color: var(--destaque);
  font-size: 1.5em;
  text-align: center;
  padding: 20px;
}

div#social{
  margin: 15px 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
}

div#social a{
  padding: 10px;
  background-color: var(--destaque);
  color: var(--texto-inverso);
  text-decoration: none;
  border-radius: 5px;
}
div#social a:hover{
  background-color: var(--destaque-inverso);
  text-decoration: underline;
  transition: 0.5s;
}

section#detalhes{
grid-column: 2;
}

article{
  background-color: var(--fundo-card);
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 8px;
}

article h2{
  color: var(--destaque);
  margin-bottom: 10px;
}

.video-container{
  position: relative;
  width: 100%;
  margin: auto;
  aspect-ratio: 16/9;
}

.video-container iframe {
  position: absolute;
  top: 0%;
  left: 0%;
  width: 100%;
  height: 100%;
  border-radius: 8px;
}
    </style>
    <link rel="stylesheet" href="estilos/style.css">
    <link rel="shortcut icon" href="favicon.svg" type="image/svg">
</head>
<body>
    <header>
        <nav id="menu">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Skills</a></li>
                <li><a href="#">Formação</a></li>
                <li><a href="#">Projetos</a></li>
                <li><a href="#">Tema</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="ficha">
            <img class="foto" src="imagens/guanabara-perfil.jpg" alt="Perfil-Guanabara">
            <h1>Gustavo-Guanabara</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut consequatur, similique accusamus cumque molestiae nesciunt excepturi at, officiis necessitatibus commodi voluptatibus. Provident assumenda quas eveniet repellat ab. Consequatur, ipsum error?
            Id, ratione harum! Tenetur nesciunt architecto magni accusantium error culpa molestias corrupti inventore, quo est vitae repudiandae quidem sed. Explicabo impedit omnis qui temporibus voluptatem assumenda perspiciatis facere, dolore aspernatur.</p>

            <div id="social">
                <a href="https://www.linkedin.com/in/guanabara/" target="_blank" rel="nofollow">Linkedin</a>
                <a href="https://github.com/gustavoguanabara" target="_blank" rel="nofollow">Git-hub</a>
                <a href="https://www.youtube.com/cursoemvideo" target="_blank" rel="nofollow">Youtube</a>
                <a href="https://www.instragam.com/gustavoguanabara" target="_blank" rel="nofollow">Instagram</a>
                <a href="https://www.cursoemvideo.com/">Site</a>
            </div>
        </section>

        <section id="detalhes">
            <h2>Deixeme apresentar</h2>
            <article id="video">
                <div class="video-container">
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/vl0eatPehLs?si=5gl9MB2ITrv7E5YJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                </div> 
            </article> <!-- Fim Article#video-->
            
            <article id="Ideias">
                <h2>Minhas Ideias</h2>
            </article><!--Fim Article-ideias-->
            
            <article id="Formacao">
                <h2>Minhas Formacoes</h2>
            </article> <!--FIm Article-formacao-->

            <article id="Projetos">
                <h2>Meus projetos</h2>
            </article> <!--Fim Article-projetos-->
        </section>

    </main>

    <footer>

    </footer>
    
    <script src="scripts/script.js"></script>
</body>
</html>
