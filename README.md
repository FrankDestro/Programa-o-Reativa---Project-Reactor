# Programação Reativa - Project Reactor 

### Conceitos 
* Sistema Reativo vs Programação Reativa
* Fluxo sincrono vs Fluxo Assincrono vs Não bloqueante

#### Sistema Reativo 🖥️⚡
- É a **arquitetura do sistema**.
- Define como o sistema reage a eventos de forma:
  - **Responsiva**: responde rapidamente.
  - **Resiliente**: continua funcionando mesmo em falhas.
  - **Elástica**: escala conforme a demanda.
  - **Orientada a mensagens**: comunicação assíncrona entre componentes.
<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/fe0a2865-abcf-40f9-8273-fc8b8463c014" /> 

#### Sistema tradicional 🖥️
<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/25c33fa8-2570-4061-b327-af3196a0e931" />

#### Programação Reativa 🖥️⚡
- É o **paradigma de programação**.
- Permite escrever código que reage a **fluxos de dados e eventos**.
- Características:
  - Fluxos assíncronos.
  - Transformações e filtros de dados (map, filter, reduce).
  - Não bloqueante (backpressure para controlar carga).


### Fluxo síncrono: 
Execução sequencial de tarefas, aguardando a conclusão de cada uma antes de continuar para a próxima.

<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/1a3a68fc-70b1-484e-8b50-fd723ad5f513" />

### Fluxo assíncrono:
Execução simultânea de tarefas, permitindo paralelismo.

<img width="640" height="360" alt="image" src="https://github.com/user-attachments/assets/7dc14394-866a-428b-87d4-63a84f1bb19c" />

Obs. Varias threads são executada em paralelo ao final da thread 0 o fluxo é completado!


### Fluxo assíncrono e não bloqueante : Uso do event loop single thread
<img width="1807" height="751" alt="image" src="https://github.com/user-attachments/assets/b2d54730-9f6a-4686-89ae-195d1329f736" />

### Não bloqueante: 
Capacidade de um programa continuar a execução sem ser bloqueado por uma outra tarefa. No Project Reactor, o mecanismo conhecido como Event Loop otimiza o uso das threads.

### Backpressure: 
Mecanismo de controle para lidar com a discrepância de velocidade entre a produção e consumo de dados.
Em programação reativa, backpressure (ou contrapressão) é um mecanismo que impede que um produtor de dados envie dados mais rápido do que o consumidor consegue processar, evitando sobrecarga, perda de dados e falhas no sistema. Ele permite que o consumidor sinalize ao produtor a sua capacidade de processamento e controle a vazão, mantendo o fluxo de dados equilibrado e eficiente. 

### Programção funcional vs Programação não funcional 

<img width="1347" height="898" alt="image" src="https://github.com/user-attachments/assets/1cbe0de2-2079-4348-a540-74e113633fc9" />

## Complemento. 
### Manifesto Reativo 
https://reactivemanifesto.org/
