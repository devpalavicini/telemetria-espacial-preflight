# telemetria-espacial-preflight
Simulador em Python da checagem final pré-decolagem de um veículo espacial. O sistema analisa dados em tempo real (temperaturas, pressão, integridade e energia), calcula a autonomia da missão e decide se o lançamento é seguro (PRONTO PARA DECOLAR) ou se deve ser interrompido (DECOLAGEM ABORTADA).

Sistema de verificação de telemetria pré-decolagem

Sobre o projeto:

Esse projeto simula o sistema de verificação pré-decolagem (pre-flight check) de uma nave, verificando dados cruciais para uma decolagem segura, como temperatura externa e interna, garantindo a segurança da tripulação e da nave antes da decolagem, emitindo o status de autorização "PRONTO PARA DECOLAR" ou o status de cancelamento da viagem "DECOLAGEM ABORTADA".

Parâmetros de telemetria:
- Temperatura interna: 18C° a 25C°
- Temperatura externa: 20C° a 30C°
- Integridade estrutural: (0/ 1)
- Nível de energia: >= 80%
- Pressão dos tanques: 
- Status dos módulos: Todos operacionais (True)

Tecnologias utilizadas:
- Linguagem: Python
- Ambiente: Jupyter Notebook
- Bibliotecas: random (simulação de dados)
