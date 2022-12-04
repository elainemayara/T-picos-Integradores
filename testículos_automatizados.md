1 - Porque devemos fazer testes automatizados nas aplicações que desenvolvemos?

R - Aumenta a eficiência do processo de testagem,
o teste automatizado economiza tempo e permite capturar possíveis bugs com mais detalhes,
aumentando assim a eficiência do teste e da entrega final.

2 - O que são testes unitários?

R - O teste unitário é uma verificação feita com uma pequena porção de código, uma unidade de um software. Ou seja,
é diferente do teste geral, que se dedica a atestar o fluxo do sistema, com as funcionalidades principais. No unitário, cada parte do sistema ganha uma atenção devida
e detalhada, de modo a otimizar o processo de identificação de erros. O objetivo é ajudar a rastrear os bugs e impedir que eles retornem depois que alterações forem 
feitas no produto.

3 - O que são testes automatizados? 

R - O teste automatizado é um recurso muito utilizado no desenvolvimento de software, onde o principal objetivo é facilitar a etapa de teste por meio de ferramentas
específicas. Dessa forma, é possível pré-programar o que será testado para então só agir quando for necessário.

4 - Escolha uma pirâmide de testes e descreva com suas palavras cada sessão da pirâmide. 

R - Modelo proposto por Mike Cohn, em que ele definiu três camadas para uma suíte
de testes, sendo elas: Unit Tests, Service Tests e UI Tests. Testes de Unidade Os testes de unidade correspondem às camadas na base da pirâmide de testes e devem ser 
considerados os pilares dessa estrutura. Essa é a camada que mais testaremos e visa isolar a menor parte testável do software, removendo qualquer interação externa real
e garantindo que ele funcione de acordo com a especificação. A analogia com conceitos mais comuns, como orientação a objetos, é como testar os métodos públicos de uma
classe para garantir que a entrada e a saída atendam às expectativas. Existem algumas técnicas que facilitam o isolamento de classes e podem ser utilizadas de acordo 
com o resultado desejado, como: spoofs, mocks, spies, stubs e dummies. Podemos considerar os testes de unidade como a linha de frente da nossa estratégia de teste. 
Eles são os primeiros a serem implantados e cada unidade tem papel fundamental na correção de erros e prevenção de falhas. Se bem implementados, também servem de guia 
para quem quer entender como o projeto funciona e para novos desenvolvedores que ingressam no projeto. Esses testes tendem a ser menores, menos complexos, cobrem a
maioria das linhas de código, têm tempos de execução rápidos e detectam bugs facilmente. Testes de Integração Pense no seguinte cenário: temos pneus de bicicleta, 
cabine de caminhão e suspensão de carro. Individualmente todos funcionam muito bem e atendem suas especificações, mas quando integrados os pneus não cabem na suspensão 
do carro e a cabine também não cabe na suspensão. Não funciona. Essa bagunça precisa ser organizada, e testes de integração são usados para resolver esse tipo de problema. 
Enquanto garantimos que as unidades de software funcionem de forma independente, também é necessário garantir que elas mantenham sua funcionalidade de acordo com seus 
requisitos quando integradas. Isso significa que precisamos garantir que as unidades trabalhem juntas e com suas dependências. Os testes de integração estão na camada 
central da pirâmide e, ao contrário dos testes de unidade, possuem um número menor de casos de teste, geralmente levam mais tempo, exigem um ambiente mais complexo e
dependem de interações externas, tornando-os mais complexos, eles geralmente têm um tempo de implementação mais longo. Devido à sua complexidade, uma boa estratégia para
esta camada é verificar cenários que não podem ser cobertos por testes de unidade e não fazem muito sentido em testes end-to-end. Identificar módulos sensíveis à operação
do sistema e integração com serviços externos é uma boa estratégia para identificar possíveis casos de teste para esta camada, abrangendo ainda mais a cobertura do código 
e minimizando a possibilidade de erros. Eles costumam ser usados para verificar a comunicação com bancos de dados, micros serviços, sistemas de arquivos, APIs externas e 
os próprios controladores do projeto. Testes de Ponta a Ponta Os testes de ponta a ponta estão no topo da pirâmide e visam testar todo o fluxo de uma aplicação do início 
ao fim, tentando simular a rotina do usuário dentro daquela aplicação e verificar se ela responde de acordo com os requisitos do projeto.
