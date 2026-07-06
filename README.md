a)  nome e número de matrícula dos autores;

MEMBROS DA EQUIPE: ROGÉRIO CORRÊA DE CAMPOS - MATRÍCULA: 26180315, MATHEUS RAUPP DE MELO, MATRÍCULA: 26104502, LUCAS GARIA VIEIRO, MATRÍCULA: 26103977

b)  descrição geral do sistema; 

O PetMatch é um sistema de adoção de animais desenvolvido em Java para a disciplina de Fundamentos da Programação da PUCRS. Executado inteiramente pelo terminal, o sistema tem como objetivo aproximar adotantes e animais por meio de uma análise de compatibilidade baseada no perfil de cada usuário.

A aplicação permite que o usuário realize seu cadastro, visualize e atualize suas informações, consulte os animais disponíveis para adoção e pesquise pets utilizando filtros específicos. Além disso, o sistema conta com a funcionalidade PetMatch, que compara as respostas de um questionário preenchido pelo adotante com as características cadastradas de cada animal, exibindo o nome de todos os pets disponíveis acompanhado de seu respectivo nível de compatibilidade.

Os animais disponíveis para adoção são previamente cadastrados no sistema e não podem ser alterados pelos usuários. Atualmente, o sistema suporta o cadastro de até 10 usuários e trabalha com um banco fixo de 10 animais, sendo uma aplicação voltada para demonstrar os conceitos de programação orientada a objetos, manipulação de vetores, métodos, encapsulamento e interação com o usuário por meio do console.

c)  imagem do diagrama de classes e com explicação das classes e composição entre elas; ![Diagrama](Diagramadeclasses)


O diagrama de classes representa a estrutura do sistema de adoção de pets e o relacionamento entre suas principais classes. A classe Pessoa possui uma relação de composição com Endereco, pois cada pessoa possui um endereço associado. A classe Pessoa também utiliza a classe Animal para calcular a compatibilidade entre o perfil do adotante e o pet. A classe BancoDeAnimais mantém um vetor com todos os objetos da classe Animal disponíveis para adoção. A classe Registros é responsável por criar e retornar um objeto Pessoa a partir das informações inseridas pelo usuário. Por fim, a classe APP coordena o funcionamento do sistema, utilizando as demais classes para realizar o cadastro, pesquisas, alterações e o PetMatch.

Observação: Na classe Animal, os métodos getters e setters foram representados apenas como "getters e setters" no diagrama para evitar excesso de linhas e manter a leitura mais organizada, já que eles seguem o padrão convencional de acesso aos atributos e não alteram a estrutura do sistema.

d) quais foram as fontes de consulta utilizadas e links de acesso; 

Durante o desenvolvimento do projeto, foram utilizadas como fontes de consulta o ChatGPT (OpenAI), para auxílio na revisão de conceitos, esclarecimento de dúvidas e apoio à implementação do código, além dos materiais disponibilizados pela professora na plataforma Moodle, utilizados como base para o desenvolvimento do trabalho.

e) informações detalhadas sobre uso de IA; 

e)

e.1) Ferramentas de IA utilizadas

Durante o desenvolvimento do projeto foi utilizada exclusivamente a ferramenta ChatGPT (OpenAI) como apoio ao aprendizado e ao desenvolvimento da aplicação.

e.2 ) Prompts utilizados e situações de uso

Esclarecimento de dúvidas sobre a linguagem Java e conceitos de Programação Orientada a Objetos;
Explicação do funcionamento de estruturas como vetores, métodos, classes, construtores, encapsulamento e passagem de parâmetros;
Auxílio na organização das classes e dos métodos do projeto;
Discussão da lógica utilizada na funcionalidade PetMatch
Identificação e correção de erros encontrados durante a implementação;
Revisão do código para entender se alguma funcionalidade ou "arquitetura" poderia ser muito melhorada

Exemplos de prompts utilizados:

"Por que este método não está funcionando?"
"Como organizar melhor essa classe?"
"Qual o problema neste trecho de código?"
"Como calcular a compatibilidade entre uma pessoa e um animal?"
"Como evitar este erro em Java?"

e.3) Principais respostas obtidas com apoio da IA

Explicações sobre conceitos da linguagem Java;
Sugestões de melhorias na organização do código;
Auxílio na identificação da causa de erros de compilação e execução;
Orientações para implementar corretamente a lógica do sistema de compatibilidade entre usuários e animais;

As conversas foram utilizadas apenas durante o desenvolvimento e não foram registradas por meio de links específicos.

e.4) Como o grupo verificou as recomendações e os códigos gerados

Todas as sugestões fornecidas pelo ChatGPT foram analisadas pelo grupo antes de serem utilizadas. Os códigos foram implementados manualmente, compilados e testados na aplicação para verificar seu funcionamento. Quando alguma resposta não era compreendida ou não produzia o resultado esperado, novas perguntas eram realizadas até que o grupo entendesse a solução proposta.

e.5) O que foi aceito, alterado ou descartado das respostas da IA

As respostas foram utilizadas apenas como apoio ao desenvolvimento. Diversas sugestões foram adaptadas para atender à estrutura adotada pelo projeto, mantendo a organização definida pelo grupo. Algumas recomendações foram descartadas quando não eram compatíveis com os requisitos do trabalho ou quando existiam soluções consideradas mais adequadas após análise e testes realizados pela equipe.

f) dificuldades encontradas e como as foram superadas; A maior dificuldade do nosso projeto foi desenvolver a lógica do PetMatch. Precisávamos criar uma forma de comparar o perfil do usuário com as características de cada animal para recomendar aqueles que fossem mais compatíveis. Durante o desenvolvimento, percebemos que algumas ideias precisavam ser ajustadas, como a pergunta sobre necessidades especiais, que inicialmente era de 1 a 5 e depois passou a ser respondida com 'Sim' ou 'Não'. Isso exigiu mudanças na lógica de compatibilidade e em outras partes do sistema. Também tivemos desafios para integrar todas as classes, garantindo que elas se comunicassem corretamente, além de implementar funcionalidades como impedir cadastros duplicados e permitir a pesquisa de pets por características. Apesar dessas dificuldades, conseguimos organizar o código, distribuir bem as responsabilidades entre as classes e desenvolver um sistema funcional que atende aos objetivos do projeto. Nós superamos esses problemas em call no Discord e com auxílio de IA, como por exemplo na classe Registros, dentro do metódo registrarPessoa, em que a leitura do scanner doubleMetragem estava dando erro e a IA sugeriu um parseDouble como solução e funcionou.

g) divisão de tarefas entre os integrantes do grupo; 

Rogério:
Classe Pessoa, método de compatibilidade (funcionalidade inovadora)

Matheus:
Classe endereço, Menu de interação da Main, funcionalidade de registro

Lucas:
Classe Animal, banco de animais, diagrama de classes

h) lições aprendidas com o trabalho; Com esse trabalho, aprendemos na prática como funciona a programação orientada a objetos e a importância de dividir um sistema em classes, onde cada uma possui uma responsabilidade específica. Também entendemos melhor conceitos como encapsulamento, construtores, getters e setters, além da utilização de vetores de objetos para armazenar e manipular informações. Outro aprendizado importante foi perceber que, durante o desenvolvimento, é comum precisar revisar e adaptar a lógica do sistema para atender melhor aos requisitos, como aconteceu com o cálculo de compatibilidade. Por fim, aprendemos a importância de testar o sistema constantemente, corrigir erros de integração entre as classes e trabalhar de forma organizada para chegar a um resultado funcional.
