# Mateus Ferreira

>Objetivo: Vaga para Pessoa Desenvolvedora no time de Tecnologia do Nexo.


### Sobre mim 

Tenho 25 anos, natural do interior de São Paulo e, desde Setembro de 2020, me aventuro no mundo da programação e desenvolvimento. Sou estudante de Análise e Desenvolvimento de Sistema pela FIAP e desenvolvo pequenos projetos open-source focados em desenvolvimento web front-end. Paralelo a isto, também carrego um diploma em Jornalismo, tendo me formado pela Universidade Federal de Uberlândia em 2017. Atuei como freelancer em tempo integral até final de 2020 e neste ano reduzi pela metade o fluxo de trabalho que tinha nesta área, para poder me dedicar ao aprendizado da programação. Convido-os acessar meu [LinkedIn](https://www.linkedin.com/in/mateus-ferreira-3315a1109/) caso tenham interesse em entender melhor meu caminho profissional até aqui 

## Seu desafio

### Criar e hospedar um aplicativo React com AWS Amplify CLI

**Resultado: confira o [repositório](https://github.com/mateusasferreira/news-app) no github e/ou acesse o [domínio](https://dev.d2b1d7p16viavz.amplifyapp.com/) onde está hospedado.**

>Obs: O app usa uma chave para teste de uma api externa, caso o conteúdo esteja indisponível, provavelmente o limite diário de requisições foi atingido, e neste caso seria ideal acessar de novo no dia seguinte. Caso tenham algum problema, por favor entrem em contato comigo (11 992904502)

Desenvolvi o protótipo de um site de notícias com backend e api próprios (apesar dos dados da api serem providos de uma api externa). A princípio, minha intenção era realizar o desafio de implementar um app React com o console do AWS Amplify, porém fui "seduzido" pelo workflow do AWS Amplify CLI. O app funcionaria da mesma maneira somente consumindo uma API externa, sem a necessidade de um backend. Porém, quis experimentar como é criar uma api pelo AWS Amplify, dando também a possibilidade de escalar a aplicação incluindo funções de post, para que seja possível cadastrar notícias e conteúdos próprios. 

#### Desafios que tive durante o desenvolvimento:  

- O primeiro totalmente operacional: não consegui verificar de primeira minha conta recém-criada na AWS (algum problema com o sistema de verificação deles). Entrei em contato com atendimento, e uma pessoa do time de atendimento da AWS dos EUA me ligou para confirmar o número e em 24h o problema foi resolvido. 

- Enquanto não tinha a conta confirmada, comecei a desenvolver o app com create-react-app e o desafio foi encontrar uma API externa que atendesse minha necessidade. A princípio optei por uma que só dava direito a 500 resquests mensais no plano gratuito, e depois optei pela [NewsApi](https://newsapi.org/) que dá direito a 100 requests diários, o que considerei suficiente para testes. 

- Tive que me interar sobre a criação de apis com Amplify CLI e Lambda functions, ainda quero me aprofundar mais nisso mas o primeiro contato foi tranquilo. 

- Tive alguma dificuldade no início para assimilar a linguagem backend criada, a qual não estou muito habituado, e fazer as alterações necessárias. Mais especificamente em como o código poderia dar opção de fazer querys no consumo pelo front. Cheguei na seguinte solução: 

```javascript 
var axios = require('axios')
app.get('/articles', function(req, res) {
  const params = req.query
  axios.get('https://newsapi.org/v2/top-headlines',{
    params: {
      category: params.category,
      country: "us",
      apiKey: "febafaab9d9d40f781cb70b922d4bc2b",
      sort: "publishedAt",
      pageSize: "9",
      language: "en"
    }
  })
    .then(response => {
      const articles = response.data.articles
      res.json({
        error: null, 
        articles
      })
    })     
    .catch(err => {
      res.json({
        error: err,
        articles: null
      })
    })
  });

```
- Por último, fiz o deploy e hosting pela linha de comando. Não fiquei tão satisfeito com o nome do domíno, gerado automaticamente. Talvez fazendo o deploy pelo repositório do Github no console do AWS Amplify ficaria mais "apresentável", mas considerei isso só um detalhe. 

>A experiência em si foi muito interessante e pretendo continuar estudando este padrão serverless, cloud e as funcionalidades da AWS. 



----

### Informações Básicas

-  **Mateus Augusto Silva Ferreira**
- **Ele/dele**
- **[Github](https://github.com/mateusasferreira) | [LinkedIn](https://www.linkedin.com/in/mateus-ferreira-3315a1109/) | [Currículo](https://www.linkedin.com/in/mateus-ferreira-3315a1109/detail/overlay-view/urn:li:fsd_profileTreasuryMedia:(ACoAABtRPpUBE5unhIh7oKEWxUJ8W18JLMlf6mM,1635458012199)/)**


- Inspiração: cite pessoas que te inspiram - Não precisa ser necessariamente da área de tecnologia

> Essa é sempre uma pergunta difícil para mim, minha inspiração por pessoas surge de forma ocasional, e quase sempre por pessoas do meu próprio convívio. Talvez as características quem mais me inspiro sejam a sinceridade, respeito ao próximo, e pensamento livre. Mas prefiro não me arriscar com nenhum nome. 

- Tecnologia com a qual mais gostaria de trabalhar: 

>No momento, React. E como linguagem, JavaScript. Também tenho praticado TypeScript, se tiverem interesse em checar meu último projeto utilizando a linguagem, aqui vai o [link](https://github.com/mateusasferreira/checkout-form).

- Possui algum projeto que gostaria de executar?
>Gostaria de executar algum projeto do zero com Next.Js (já tive contato com a ferramenta em treinamentos online), penso em algo como um protótipo de e-commerce ou blog. 

- "Uma democracia saudável requer jornalismo crítico, que examine e monitore qualquer governo, uma vez que estamos todos sujeitos a prestar contas." Qual a sua visão do jornalismo e seu papel hoje na sociedade em meio ao cenário de fake news?

> Acredito que o jornalismo deve estar sempre alinhado com o interesse público em detrimento do privado e sempre vigilante das instituições democráticas. Não há o que se discutir quanto ao "fato" ser o ativo fundamental do jornalismo. Já no lado mais subjetivo e opinativo da narrativa jornalística, acredito que os pilares devem ser a responsabilidade social, a consonância com os direitos humanos e demais agendas que surgiram a partir dela, e o respeito ao regime democrático. 

- E-mail e celular para contato. Iremos, preferencialmente, manter toda a comunicação por e-mail

> Email: mateusaugustosferreira@hotmail.com

> Celular/Wpp: (11) 992904502

Por favor, caso esteja de acordo, declare seu consentimento de compartilhamento de dados para os propósitos desta chamada:

- [X] Eu, Mateus Ferreira, expresso meu pleno consentimento em compartilhar estes dados para fins do processo seletivo do Nexo Jornal, e estou ciente de que poderei, a qualquer momento, solicitar a exclusão dos meus dados pessoais, de acordo com a [LGPD](http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm), notificando a equipe responsável pela guarda desses dados por meio do email _tecnologia@nexojornal.com.br_ que fará a eliminação de seus dados pessoais guardados dentro dos prazos legais.


**Por fim, queria elogiar o formato desta primeira etapa de seleção, extremamente empolgante. E agradecer pela oportunidade, que foi de grande importância também para o meu aprendizado.**

**O Nexo é um meio que admiro desde minha época como estudante de jornalismo. Poder contribuir de alguma forma para um meio tão importante seria muito gratificante para mim.**

**Espero falar com vocês em breve. Um abraço!** 