# Qual a função do "head" no HTML?
    O head tem como função definir as configurações de um site.
    É no head onde definimos o titulo do site, assim como tambem fazemos a linkagem de arquivos css ou até mesmo javascript.
    É no head onde definimos algumas configurações para auxilio de responsividade e tambem definimos configuraçoes de SEO (através das meta tags definindo "descriptions", "keywords", "robots", etc..);

# Quando uma página é criada, ela automaticamente se adapta a todos os tipos de tela? Por que?
    Não. Para que uma pagina se adapte a todos os tipos de telas, é necessário criar configurações de responsividade tais como: -    Usando uma meta tag "viewport" (definindo que a lagura da tela será igual a lagura do dispositivo);
    -    Criando regras de adaptaçao para os itens necessários atráves de media query (É onde definimos que a de e até determinado tamanho de tela, tais componentes irão receber outras propriedades de tamanho, largura, altura, display, etc.. para que assim.. o mesmo se adapte a aquele tamanho de tela );
    
# O código HTML e CSS é renderizado no servidor e repassado para o navegador em forma de imagem?
    Não. O HTML e CSS são armazenados no servidor. Quando acessamos um site na verdade estamos fazendo uma requisição ao servidor daquele site através do DNS do mesmo. Que retorna os Arquivos HTMl e CSS. O responsavel pela renderização é o proprio navegador no lado do cliente que ao receber o arquivo HTML e CSS ele processa esse arquivo retornando todo o conteudo ao clietne. 

# Qual a função das tags H (h1, h2, h3, etc) no HTML?
    As tags "H" são tags usadas para definir titulos em uma pagina. 
    Além de definir titulos, sao usadas como ferramentas de SEO, onde o h1 dita o titulo principal desta página (por esse motivo é aconselhavel que haja apena um h1 por página), e de acordo com que aumente a tag (h2, h3.. h6) tem menor prioridade.
# O que é SEO e como funciona?
    O SEO (Search Engine Optimization) ou Otimização para Motor de Busca, isto é, um conjunto de ferramentas ou configuração que usamos para melhorar o posicionamento da pagina nos motores de busca (Google, Bing, etc...);
    Fazemos isso por exemplo, usando tags semanticas como:
        h1 - Onde dizemos qual o assunto principal daquela pagina;
        article - Artigos ou posts se for um site de noticias ou blog;
        header - Onde se situa o cabeçalho da pagina
        nav - Onde se situa o menu de navegação
    E através de meta tags onde podemos descrever diretamente uma descrição do que se trata a pagina (<meta name: "description"... />) ou as keywords dela (<meta description name:"keywords" ... />);

    E quando um motor de busca puxa/faz a requisição da nossa pagina ao servidor para apresentar ao cliente, ele faz uma analise de todo o HTML. Nessa analise ele verifica todo o conteudo do HTML e através das tags semanticas e meta tags ele te posiciona para um publico alvo e direciona a sua pagina para um nixo expecifico ou separado para determinados tipos de busca.

# O uso de media query é obrigatório em todas as páginas?
    Não. O media query é usado apenas quando queremos que a página se adapte em outros tamanhos de tela ou que quando der o comando para imprimir aquela página, ela seja impressa de uma maneira em expecifico (se bordas ou margens por exemplo);

# Qual a diferença entre CSS Inline e CSS em um arquivo?
    A execução e o resultado final será o mesmo. Porém com um CSS em um arquivo separado se torna muito mais facil a manutenção e organização do código.

# Como criar animações no CSS? Dê um exemplo.
    @keyframes changeColor {
        0% { background-color: red; }
        25% { background-color: green; }
        50% { background-color: blue; }
        75% { background-color: white; }
        100% { background-color: yellow; }
    }

    div {
        width: 100px;
        height: 100px;
        background-color: #fff;
        animation-name: changeColor;
        animation-duration: 5s;
        animation-delay: 1s;
    }
# Qual a diferença entre class e ID no CSS?
    O ID é aconselhado que se use apenas em um elemento;
    A class já se pode usar em mais de um elemento;

    <div id="container">
        <div class="content" >...</div>
        <div class="content" >...</div>
        <div class="content" >...</div>
    </div>

    CSS
        #container {
            width: 100%;
            height: 100vh;
        }
        .content {
            width: 100%;
            height: 100px;
            background-color: #ff0000;
        }
        
# Quais os diferentes tipos de seletores CSS?
    Os principais tipos de seletores CSS são:
        - tag
        - class
        - id
        - atributo