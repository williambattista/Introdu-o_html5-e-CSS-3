



# MEU PRIMEIRO CONTATO

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>William Batista</title>
        <link rel="stylesheet" href="style.css">

    </head>
    
    <body>
        <header>
            <!--img adiciona uma imagem, já alt adiciona uma descrição para a imagem-->
            <img src="Foto de Perfil.png" alt="Foto do rosto do William Batista" class="photo">
            <!--h1 relaciona ordem de título e tamanho (só pode haver um h1)-->
            <h1 id="title">William Batista</h1> <!--id é utilizado apenas uma vez-->
        </header>
        <section>
            <header>
                <h2 class="subtitle">Desenvolvimento em HTML5 e CSS 3</h2> <!--class define a classe-->
            </header>
            <article class="post">
                <header>
                    <h3 class="post_title">Post #1</h3>
                    <img src="Imagem_post.jpg" alt="Imagem ilustrativa do código HTML" class="post_image">
                </header>
                <!--p adiciona um texto-->
                <p class="post_content">
                    HTML (HyperText Markup Language) is the most basic 
                    building block of the Web. It defines the meaning and structure 
                    of web content. Other technologies besides HTML are generally used to 
                    describe a web page's appearance/presentation <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank">(CSS)</a>or 
                    functionality/behavior <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">(JavaScript)</a>.
                <!--<a href> adiciona um link e target="_blank abre uma nova aba-->
                    "Hypertext" refers to links that connect web pages to one another, either 
                    within a single website or between websites. Links are a fundamental aspect 
                    of the Web. By uploading content to the Internet and linking it to pages created by 
                    other people, you become an active participant in the World Wide Web.
                </p>                
            </article>
        </section>
        <footer>
            <!--<ul> cria uma lista sem criterio de ordem se <ol> cria-se uma lista ordenada-->
            <lu class="contact_list">
            <!--<li> cria um item da lista-->
                <li>
                    <a href="mailto:williambatsantos4@gmail.com" target="_blank">williambatsantos4@gmail</a>
                </li>
                <li>
                    <a href="https://www.linkedin.com/in/williambatista96/" target="_blank">Linkedin</a>
                </li>
                <li>
                    <a href="https://github.com/williambattista" target="_blank">GitHub</a>
                </li>
            </lu>
        </footer>
    </body>
</html>
CSS 3

body {
    background: #f7f7f7;
    font-family:  Verdana;
    /*width: 900px; /*largura para o body*/
    max-width: 900px; /*a largra máxima do body, é interessante quando a tela for menor*/
    margin: auto; /*cria um espaçamento automatico para alinhar o conteúdo ao centro*/
}
.photo {
    border-radius: 50%; /*deixa a foto em uma area circular*/
    border: solid #505050;
}

#title, .subtitle, .post_title {
    color: #505050
    
}
#title {
    font-size: 40px;
    text-transform: uppercase; /*deixa em caixa alta*/
    color: #505050;
}
a {
    text-decoration: line-through; /*coloca uma linha ao centro*/
    color: #505050;
}
.post_title {
    font-size: 16px; /* tamanho do elemento*/   
    font-style: italic; /*estilo da fonte*/
    margin: 0;
    margin-bottom: 15px;
}

.post {
    background: #fff;
    padding: 15px; /*espaçamento entre a borda e o conteúdo*/
    border:2px solid #505050;
    margin-bottom: 15px; /*magem*/
    border-radius: 5px; /*arrendondar as bordas*/
}
.post_content {
    margin: 0;
    margin-bottom: 15px;
    text-transform: capitalize; /*coloca a primeira letra em caixa alta*/
    text-align: justify; /*alinha o texto*/
}
.post_image {
    margin-bottom: 15px; /* adicionei 15px abaixo da imagem*/
    width: 100%; /*largura que respeita os limites do body*/
}
.contact_list {
    list-style-type: none; /*remove os itens*/
    padding-left: 15px;

}
.contact_list li a { /* vemos aqui que o item <li> e a âncora <a> estão dentro de <lu>
    então podemos estilizar dessa forma apenas essas partes*/
    text-decoration: none; /*retira a formatação anterior*/
    
}