![UsuCampeão](logo.png)

# USUCAMPEÃO Tecnologia em Regularização Imobiliária

Somos mais que uma Startup de regularização de imóveis, nascemos para resolver um problema social que atinge mais de 50% da população brasileira.

Através da inovação, execução de qualidade e baixo custo realizamos o sonho da propriedade regularizada.

Nosso propósito é gerar segurança jurídica e #prosperidade a todas as pessoas.

*Venha fazer parte deste time CAMPEÃO!!!*

## Desenvolvedor Front-End

Então, quer dizer que você gosta de desafios e quer se tornar um desenvolvedor front-end na UsuCampeão? Está no lugar certo!

Este teste faz parte do nosso processo de seleção e é a sua chance de nos mostrar todo o seu conhecimento como desenvolvedor front-end com angular. Este teste está dividido em duas etapas:

1. Responder um questionário sobre HTML, CSS, JavaScript e Angular
1. Desenvolver uma aplicação simples, demonstrando seu conhecimento na prática

Daremos um feedback a todos os que fizerem o Pull Request.

O questionário e a especificação da aplicação estão logo abaixo.

A sua entrega será feita através de um Pull Request nesse repositório. Faça um fork do repositório, implemente o seu código, responda as questões no README.md e faça um pull request. Sinta-se a vontade para colocar quaisquer outras informações que você considere pertinente no README.

### Instruções:

1. Faça um fork deste repositório;
1. Responda as questões no README.md - caso prefira, podemos conversar sobre elas na entrevista;
1. Construa uma aplicação conforme solicitado, utilizando HTML, CSS e Angular;
1. Adicione quaisquer informações adicionais para executar sua aplicação no README.md;
1. Após terminar, submeta um pull request e aguarde seu feedback.

**PS:** Utilizamos este mesmo testes para os níveis (**júnior**, **pleno** ou **sênior**), apenas adequando o nível de exigência na avaliação de acordo com o perfil da vaga.



### Como rodar o projeto!
Baixe o projeto, entre nele pelo cmd ou git, utilize o npm install e após use o ng serve, agora se divirta com sua nova pokedex.


### Questionário

1. O que são ``components`` e ``directives`` e quais as difenças entre eles? Dê alguns exemplos de utilização.
>Components e Directives são usadas para o reuso de códigos e a forma de passar comportamentos para o HTML, neste caso usando a linguagem JavaScript. Considerando que são "tradutoras" de comportamentos, elas se diferenciam quanto ao uso. Directives passam comportamentos diretos para a aplicação, mas não possui uma view, isso implica num tempo menor de resposta para as solicitações da aplicação, diferentemente de components, várias directives podem ser passadas em um mesmo elemento. Já o components apresenta ao usuário uma página para a visualização das ações.
2. O que são ``services``? Dê alguns exemplos de utilização.
>Uma Classe da aplicação que pode ser acessado por quaisquer componentes descritos no projeto, utilizado sempre que é necessário criar uma estrutura lógica que precisará ser acessada em outras partes do projeto. Um exemplo direto é este projeto 'PokeApp', projeto o qual fazemos requests para uma API. Considerando que esses dados devem estar disponíveis em toda a aplicação, a função é criada dentro de uma service.
3. O que são ``pipes``? Dê alguns exemplos de utilização.
>Pipes são funções que tem o propósito de formatar ou filtrar dados da aplicação de forma simples e rápida. Exemplos comuns são {{ qualquerCoisa | uppercase }} - transforma a string em maiúscula, {{ qualquerCoisa | titlecase }} - transforma o primeiro carácter em maiúscula. É possível também criar pipes para formatar dados de qualquer maneira.
4. O que é ``data-binding`` e quais os tipos que o Angular dá suporte?
>Data binding é a capacidade de conectar os dados de uma view com uma Classe ou um Model. Basicamente feito em duas formas: 'One-Way data-binding' que apenas recebe informações e 'Two-Way data-binding' que interage e altera as propriedades do objeto. Ex:

>Interpolation {{ }};
Usa a propriedade de uma Classe na View. Logo, quando alguma propriedade é alterada, a view é atualizada.

>Property Binding [];
Tanto com um elemento, como com um componente, a propriedade é fixada a algum outro dado e tem seu comportamento, então, conectado.

>Event Binding ();
Passa dado de um componente filho para um pai.

>Banana in the Box [()].
Usa tanto a conexão de propriedades quanto a conexão de eventos para criar uma "conversa" da model com o template.
5. Como se adiciona um *listener* de eventos do usuário em um componente? Por exemplo, como adicionar uma função que responde a um clique de usuário?
>Usa um 'Event Binder' dentro do componente e associa este a um evento, ex:
<button (click)="funcList()">
O usuário ao clicar no botão, dispara a função funcList() dentro da Model.
6. Quais as diferenças entre ``constructor`` e ``ngOnInit``, e quando devemos usar cada um?
>O constructor é o primeiro módulo a ser carregado. Ele estrutura os comportamentos antes do ngOnInit. Este segundo faz parte do ciclo de vida do componente. Como o constructor será iniciado primeiro, nele deve conter apenas o essencial da aplicação e com a utilização do ngOnInit não necessita inicializar variáveis ou outros componentes. Isso aumenta a performance da aplicação.
7. Quais as diferenças entre ``Observables`` e ``Promises``? Como você o utilizaria cada um em um ``template``?
>Observables servem para fazer requisições durante um período do tempo, enquanto Promises lidam apenas com um evento, ou seja, em um request, um Observable irá buscar todos os requests simultaneamente, enquanto a Promise fará um de cada vez. Ao fazer uma solicitação, a Promise tem mais suporte por ser algo nativo do JavaScript, então se o request for algo simples e direto daria para usa-la, porém, se a solicitação for algo extenso, então as Observables fariam o request em menos tempo e com mais tratamento.
8. Quais as diferenças entre ``template-driven forms`` e ``reactive forms``? Como fazer validação de dados de formulário em cada caso?
>Os template-driven-forms são formulários que tem sua estrutura toda no próprio template, fazendo o controller estar praticamente vazio, porém, o código pode ficar mais complicado de se ler pela quantidade de informações inseridas, assim, tornando-se ainda mais complexo a cada validação necessária. O reactive-form tem as validações feitas no componente,ou seja, caso o template mude a validação não será afetada.
9.  Como se utiliza o ``angular router``? Quais são as formas de enviar parâmetros para uma rota?
>O angular router é utilizado para fazer a ligação entre path e o component das páginas criadas. Crie pelomenos 2 componentes para ter a rota; Insirá o Módulo de rota no 'module.ts'; Defina as rotas no módulo, ex: {path: 'detailPoke/:id', component: DetailPokeComponent}; Depois passe `routerLink` e `routerLinkActive` para o local que será feito o routing. 
10.  O que são *guards de rota* e para que são úteis?
>São serviços que fazem um gerenciamento de rotas e trata os acessos com autenticação. Sua função principal está na capacidade de proteger informações essenciais para integridade da aplicação.
11. O que é ``NgZone``? Em que momento deve ser utilizada?
>É um método que consegue rodar um bloco de código "fora" da aplicação principal do Angular. Deve ser utilizada quando algum trabalho não precisar de atualizações para o usuário ou de tratamento de erro pelo Angular.
12. O que é *injeção de dependências* e por que isso é útil? Como você realiza injeção de dependências entre módulos?
>Injeção de dependepências é a capacidade de conversar entre classes, enviando métodos e buscando. É útil pois, podemos separar o código e rodar apenas o que é necessário. Utilizamos essas injeções por meio do implemento das classes.

Ah, e a mais importante de todas: Bulbassauro, Charmander ou Squirtle? =)
>Bulbassauro é claro, sempre sendo um pokemon muito versátil em suas habilidades...

### Projeto: Criando uma Pokédex usando a PokéAPI

Pokémon é uma enorme franquia com jogos, desenhos, filmes, brinquedos e diversos produtos mundialmente conhecidos. Da [Wikipédia](https://pt.wikipedia.org/wiki/Pokémon_(série_de_jogos_eletrônicos)):

> Pokémon é uma série de jogos eletrônicos desenvolvidos pela Game Freak e publicados pela Nintendo como parte da franquia de mídia Pokémon. Lançado pela primeira vez em 1996 no Japão para o console Game Boy, a principal série de jogos de RPGs, que continuou em cada geração em portáteis da Nintendo.
> 
> Os jogos são geralmente lançados em pares - cada um com pequenas variações - com uma recriação aprimorado dos usados jogos lançados em alguns anos depois das versões originais. Enquanto a série principal consiste em RPGs, os spin-off abrangem outros gêneros, como RPG de ação, quebra-cabeça e jogos virtuais para animais de estimação.
> 
> A partir de 24 de novembro de 2017, mais de 300 milhões de jogos de Pokémon foram vendidos em todo o mundo, em 76 títulos. Isso faz de Pokémon a segunda franquia de jogos eletrônicos mais vendidas, atrás da própria franquia da Nintendo Mario.

Em 2016, a Nintendo lançou o jogo Pokémon Go, para Android e iOS, que permitia aos jogadores "caçar" Pokémons no "mundo real" através de realidade aumentada, utilizando o GPS e a câmera dos celulares dos jogadores. Seus monstrinhos capturados ficavam listados na chamada Pokédex, um acervo de Pokémons que já existia desde o primeiro jogo.

Seu objetivo, neste projeto, é criar uma Pokédex em Angular usando a PokéAPI.

A [PokéAPI](https://pokeapi.co/) é uma API aberta, sem necessidade de  disponibiliza uma API REST com, entre outras coisas, informações de todos os Pokémons até a geração 7. Você pode consultar a documentação da API [aqui](https://pokeapi.co/docs/v2).

Você é livre para montar a aplicação como quiser, mas gostaríamos de ver a listagem de todos o Pokémons, com informações básicas, em uma página inicial e detalhes do Pokémon selecionado em outra página. Como referência de layout, recomendamos que utilize as seguintes Pokédex como exemplo:

- [Pokédex oficial](https://www.pokemon.com/br/pokedex/)

(link: [https://www.pokemon.com/br/pokedex/](https://www.pokemon.com/br/pokedex/))

![Pokédex oficial](pokemon.com.png)

- [Pokedex.org](https://pokedex.org/)

(link: [https://pokedex.org/](https://pokedex.org/))

![Podedex.org](pokedex.org.png)

Temos alguns pré-requisitos:
- Utilização de Angular 8+;
- Uso de SASS/SCSS para CSS da aplicação;
- Design responsivo;
- Ah, e não se esqueça de mostrar os sprites (as imagens) de cada Pokémon!

Além disso, vamos avaliar como você organiza e documenta o projeto, e a estrutura de módulos, componentes, serviços e rotas que você criou.

Ganhe pontos extras por:
- Uso de Angular Material;
- Layout diferenciado e animações;
- Mecanismo de pesquisa;
- Cache e persistência dos dados no ``localStorage`` ou ``IndexedDB``;
- Funcionamento offline com os dados cacheados - melhor ainda se for um PWA!;
- Testes unitários e end to end;
- Scripts de deploy;
- Organização e mensagens dos commits.

E não se esqueça, bugs e exceções são como Pokémons: *Gotta catch 'em all!*

**Boa sorte! =)**
