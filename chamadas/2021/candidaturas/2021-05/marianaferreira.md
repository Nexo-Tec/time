# Mariana de Freitas Ferreira

> Sou estudante de Ciência da Computação na UFF, tenho 22 anos e faltam dois períodos para me formar. Atualmente faço estágio em desenvolvimento web com Django, lidando com levantamento de requisitos, novas funcionalidades e correção de bugs. Estou aprendendo React para ampliar meus conhecimentos no frontend e gostaria de integrar o time do Nexo para contribuir e trabalhar com algo que acredito.

## Seu desafio

O resultado pode ser acessado [aqui](https://ferreira-mariana.github.io/react-movie-search/) e o código-fonte [aqui](https://github.com/ferreira-mariana/react-movie-search).

Escolhi o desafio [Learn React in 1 Hour by Building a Movie Search App](https://www.freecodecamp.org/news/learn-react-in-1-hour-by-building-a-movie-search-app/), porque estou começando a aprender React e seria uma ótima oportunidade para fazer um projeto, além de que gosto muito de frontend e já estava mais que na hora de subir de nível para o React. 

No tutorial não ensina a iniciar o projeto, mas usei create-react-app e foi tranquilo. Percebi algumas diferenças na estrutura, resolvi seguir a base criada pelo comando por achar mais organizado e seguir o padrão, mas apaguei alguns arquivos adicionais que não iria utilizar.

Algo que também fiz diferente foi criar o componente para buscar os filmes, mas colocar o css num arquivo separado apenas para esse componente (SearchMovies.css) para facilitar o entendimento de qual css é referente a qual parte do site, mesmo que depois seja compilado tudo em um arquivo só.

Um dos momentos de dificuldade foi na consulta à API de flimes: apareceu um erro dizendo que minha chave não estava autorizada. Conferi no site e estava tudo certo. Tentei novamente e retornou a promise com status pendente, estranhei o erro ter mudado e então percebi que só tinha colocado await para fetch(url) mas não para res.json(), então o console.log cada hora exibia uma resposta diferente dependendo do tempo da requisição. Ao colocar o await, retornou os filmes.

Gostei muito da dinâmica do tutorial de propor desafios. O único que não entendi tão bem só com a explicação do tutorial foi o desafio do states, então assisti [esse vídeo](https://www.youtube.com/watch?v=4pO-HcG2igk) para entender melhor, com isso consegui realizar o desafio, mas depois com a continuação do vídeo aprendi uma sintaxe mais enxuta.

Após finalizar o tutorial, percebi um erro quando clicamos no botão de ‘search’ sem ter digitado nenhum filme. Então, tratei verificando se existem filmes antes de renderizar os cards e adicionei uma mensagem incentivando o usuário a escolher um filme caso não tenha sido digitado nenhum na busca. Além disso, alterei o layout para ficar com mais estilo de cinema.

Por fim, utilizei [esse tutorial](https://dev.to/yuribenjamin/how-to-deploy-react-app-in-github-pages-2a1f) para realizar o deploy no github pages.


----

### Informações Básicas

- Nome Completo: Mariana de Freitas Ferreira
- Pronome: ela/dela
- Se possui dev.to, bibliotecas open source, etc: Começando no [dev.to](https://dev.to/mari_dff).
- LinkedIn e link para o seu CV: [LinkedIn](https://www.linkedin.com/in/mariana-dff/) e [CV](-https://drive.google.com/file/d/1p08KwWAgG71IymStkGRXbChPVUYRUz-5/view?usp=sharing).
- Inspiração: cite pessoas que te inspiram - Não precisa ser necessariamente da área de tecnologia: Audre Lorde, Chiquinha Gonzaga e Dorothy Vaughan.
- Tecnologia com a qual mais gostaria de trabalhar: ReactJS e NodeJS, mas aberta a outras tecnologias, claro.
- Possui algum projeto que gostaria de executar?: Tenho vontade de criar um site interativo sobre educação feminista, numa vibe parecida com esse [aqui](https://ncase.me/trust/), mas ainda estou elaborando como vai ser.
- "Uma democracia saudável requer jornalismo crítico, que examine e monitore qualquer governo, uma vez que estamos todos sujeitos a prestar contas." Qual a sua visão do jornalismo e seu papel hoje na sociedade em meio ao cenário de fake news? Relate brevemente sua opinião sobre esse assunto. (Lembre-se, não há resposta correta. Toda a indústria tem discutido e debatido essas questões no momento): Acredito que educação e informação são essenciais para a construção de uma sociedade democrática. No momento atual, as fake news e a polarização estão trazendo muita desinformação e tornando o diálogo muito difícil. Para avançarmos na sociedade brasileira, é preciso que existam debates saudáveis, algo que infelizmente está diminuindo. Para chegar nas pessoas, precisamos de acessibilidade e também trazer conhecimento, uma das formas de alcançar isso é através do jornalismo.


Por favor, caso esteja de acordo, declare seu consentimento de compartilhamento de dados para os propósitos desta chamada:

- [ ] Eu, Mariana Ferreira, expresso meu pleno consentimento em compartilhar estes dados para fins do processo seletivo do Nexo Jornal, e estou ciente de que poderei, a qualquer momento, solicitar a exclusão dos meus dados pessoais, de acordo com a [LGPD](http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm), notificando a equipe responsável pela guarda desses dados por meio do email _tecnologia@nexojornal.com.br_ que fará a eliminação de seus dados pessoais guardados dentro dos prazos legais.

PS: Você pode incluir quaisquer informações extras, links e recursos que considere pertinentes para os propósitos desta chamada.
