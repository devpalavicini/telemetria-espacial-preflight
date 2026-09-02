# telemetria-espacial-preflight
Simulador em Python da checagem final pré-decolagem de um veículo espacial. O sistema analisa dados em tempo real (temperaturas, pressão, integridade e energia), calcula a autonomia da missão e decide se o lançamento é seguro (PRONTO PARA DECOLAR) ou se deve ser interrompido (DECOLAGEM ABORTADA).

Sistema de verificação de telemetria pré-decolagem

Sobre o projeto:

Esse projeto simula o sistema de verificação pré-decolagem (pre-flight check) de uma nave, verificando dados cruciais para uma decolagem segura, como temperatura externa e interna, garantindo a segurança da tripulação e da nave antes da decolagem, emitindo o status de autorização "PRONTO PARA DECOLAR" ou o status de cancelamento da viagem "DECOLAGEM ABORTADA".

Código feito em Python, contendo variáveis, if elif e else, função random e listas para que na escolha da função random na variável de status dos módulos, os valores sejam escolhidos entre True e False, com True tendo 80% de chance de ser escolhido e False tendo 20% de chance.

Os cálculos de energia foram baseados no material do capítulo 7 da fase 1, utilizando operadores e valores em variáveis, onde foi abordado o conceito da primeira e segunda leis da termodinâmica, princípios de potência e rendimento, cálculo de perdas e rendimento global.

Muitas das variáveis utilizaram a função random, sendo variáveis com valores em float (random.uniform) e as variáveis com valores inteiros (random.randint), sendo ambas definidas os valores base e valores teto a serem escolhidos. 

Todos os processos são realizados por meio de if, elif e else, checando se o valores batem com os parâmetros pré-definidos ou não. Caso os valores estejam de acordo com os parâmetros, é adicionado uma string em forma de concatenação a uma variável string com o operador relacional +=, chamada “relatorio”.
Caso os valores não estejam de acordo com os parâmetros, é adicionada outra string em forma de concatenação a variável “relatorio” e é adicionado o valor “True” a variável “testfalhou”, onde inicialmente essa variável contém o valor False, indicando que nenhum teste falhou nos processos.

Parâmetros de telemetria:
- Temperatura interna: 18C° a 25C°
- Temperatura externa: 20C° a 30C°
- Integridade estrutural: (0/ 1)
- Nível de energia: % - Autonomia restante do cálculo em kWh >= 0 
- Pressão dos tanques: 150 a 200 bar
- Status dos módulos: Todos operacionais (True)

Tecnologias utilizadas:
- Linguagem: Python
- Ambiente: Jupyter Notebook
- Bibliotecas: random (simulação de dados)
