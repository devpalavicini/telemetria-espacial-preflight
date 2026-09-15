# telemetria-espacial-preflight
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

Cálculos utilizados:
- rendimento = (energia utilizada / energia total utilizada) * 100
- energía disponivel = capacidade total * (carga atual / 100)
- energia útil = energia disponível * (rendimento / 100)
- autonomia restante = energia útil - consumo estimado para decolagem

Tecnologias utilizadas:
- Linguagem: Python
- Ambiente: Jupyter Notebook
- Bibliotecas: random (simulação de dados)

Prints da Execução:
<img width="1447" height="467" alt="image" src="https://github.com/user-attachments/assets/28bdc14b-287d-4bb3-b737-1ccecd60841c" />
<img width="1436" height="432" alt="image" src="https://github.com/user-attachments/assets/c4b97afa-41cb-4c09-8558-1b167b8c7a35" />
<img width="1447" height="433" alt="image" src="https://github.com/user-attachments/assets/d2a839b5-6d20-4ed1-bbfe-37841bba7c85" />


Como executar:
Pré requisitos: Python 3. instalado (não é necessário nenhuma biblioteca instalada)
Execução: Execute o arquivo no seu terminal
bash telemetria_espacial_preflight.py

