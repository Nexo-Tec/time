# Daniel Sarsi Orta

> Sou o Daniel, tenho 25 anos e atualmente sou estudante de graduação em Psicologia pela Universidade Federal de São João del-Rei (UFSJ). Tenho familiaridade com desenvolvimento web (front-end e back-end), a qual pude aprimorar inclusive cursando a graduação. Tenho conhecimento de HTML, CSS e JavaScript (Node.js, TypeScript, Deno), como também as mais diversas ferramentas (Vue.js, SCSS, AlpineJS, Jekyll, entre outros). Esta chamada me chamou atenção pela importância dada à narrativa como uma maneira de entender o trabalho.

## Seu desafio

Para este desafio, resolvi fazer (mais) uma versão do [Hacker News](https://news.ycombinator.com/) utilizando a [API oficial](https://github.com/HackerNews/API). Para isto, decidi utilizar Next.js e dar deploy Vercel.

:red_circle: **Live:** [https://h.sarsi.cc/](https://h.sarsi.cc/)  
:page_facing_up: **Código-fonte:** [https://github.com/danielsarsi/hacker-news](https://github.com/danielsarsi/hacker-news)

Com agora pronto, quero relatar meu trajeto, dúvidas e descobertas:

1. **Vercel é, de fato, uma boa jamstack para Next.js**  
   Em outras experiências, Netlify pareceu funcionar melhor, mas Vercel é sem estresse para dar deploy em projetos feitos com Next.js.

2. **Formatação de data sempre no server-side**  
   Inicialmente, as datas dos items eram formatadas no client-side. Porém, fica claro que é preciso um controle para qual fuso horário a data é formatada. Não podemos depender de um fuso horário certo no computador do cliente.

3. **Next.js melhorou muito ao longo dos anos**  
   Trabalhei com Vue.js (`vue-cli`) por mais tempo, mas Next.js se provou uma boa ferramente para desenvolvimento.

4. **A API pública do Hacker News me dá agonia pela quantidade de requisições que são necessárias**  
   Um item retorna todas as IDs dos comentários. Por sua vez, é preciso requisitar todos os comentários, um por um, para mostrar todos. Isso pode chegar a dar 500 requisições em um único item :man_facepalming:. Posteriormente, pensei em fazer alguma espécie de cache para diminuir as requisições.

5. **O `Incremental Static Regeneration (ISR)` é mágico :stars:**  
   A possibilidade de renderizar a página estática novamente depois de um tempo determinado on-demand abre muitos caminhos para fazer uma aplicação rápida.

6. **É importante foco para não se perder nas diversas funcionalidades de um framework**  
   Várias vezes me dei conta que estava complexificando algo que poderia ser mais simples. Otimizar e refatorar códigos, junto com bastante leitura sobre com o que trabalha, ajuda a dar foco.

7. **O rápido avanço do CSS me surpreende**  
   Nesse projeto, utilizei `text-decoration-thickness` e `text-decoration-color` pela primeira vez. Não há mais necessidade de utilizar `border-bottom` para personalizar linhas dos textos!

Obrigado pela oportunidade!

---

### Informações Básicas

- Daniel Sarsi Orta
- ele/dele
- [LinkedIn](https://www.linkedin.com/in/danielsarsi/)
- Sigmund Freud.
- Sinto-me bem confortável em trabalhar com HTML, CSS e JavaScript, como também em Next.js.
- daniel@sarsi.cc, (32) 98700-5890

> "Uma democracia saudável requer jornalismo crítico, que examine e monitore qualquer governo, uma vez que estamos todos sujeitos a prestar contas." Qual a sua visão do jornalismo e seu papel hoje na sociedade em meio ao cenário de fake news?

Apresenta-se como um desafio ao jornalismo o posicionamento editorial que coadune com nossas convicções e acordos civilizatórios. Apresentar a informação supostamente descolada da construção de uma narrativa, ou o chamado "jornalismo declaratório", fomenta uma ideia de neutralidade, como se o julgo da informação estivesse apenas a cargo do leitor. Apenas a transmissão de uma informação já a coloca em algo além do mero fato: há intenções, direcionamentos, caminhos. Como vi recentemente, se um dos lados for o fascista, o jornalista não precisa publicá-lo na capa ao lado do democrata; disto cabe a decisão editorial.

Por favor, caso esteja de acordo, declare seu consentimento de compartilhamento de dados para os propósitos desta chamada:

- [x] Eu, XXXX, expresso meu pleno consentimento em compartilhar estes dados para fins do processo seletivo do Nexo Jornal, e estou ciente de que poderei, a qualquer momento, solicitar a exclusão dos meus dados pessoais, de acordo com a [LGPD](http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm), notificando a equipe responsável pela guarda desses dados por meio do email _tecnologia@nexojornal.com.br_ que fará a eliminação de seus dados pessoais guardados dentro dos prazos legais.
