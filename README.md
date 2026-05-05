# Trabalho Prático de Teste de Software

# (1) os nomes dos membros do grupo:
Guilherme Augusto Silva Camilo

# (2) explicação do sistema
Este trabalho prático da disciplina Teste de Software trata de um estudo de caso de uma API financeira amplamente utilizada no mercado de capitais, a Alpha Vantage, 
sob a ótica da resiliência e robustez de integrações em sistemas distribuídos. 
O objetivo central é analisar **como uma aplicação cliente deve se comportar diante de falhas não determinísticas** de um **provedor de dados de terceiros** (Third-Party API), 
onde o contrato de interface é frequentemente desafiado por restrições de infraestrutura e políticas de rate limiting.
Para além da simples verificação funcional, este estudo propõe uma **avaliação empírica** de **mecanismos de tolerância a falhas**, como estratégias de Retry (recursão com controle de estado) e 
validação semântica de payloads. A relevância deste estudo para a disciplina reside na **investigação** de como o software pode manter sua **integridade** mesmo **quando o ambiente externo** (camada de transporte e serviços externos) 
**apresenta comportamentos anômalos**, como respostas parciais (truncamento de dados) ou violações de protocolo REST (ex: retorno de status code 200 para erros de aplicação).

# (3) explicação das possíveis tecnologias utilizadas
Ambiente de execução: Node.js<br>
Linguagem: JavaScript<br>
Utilização de Async/Await e Promises para o controle de fluxo de requisições e resiliência do sistema.<br>
Axios: biblioteca utilizada para realizar requisições à API<br>
Moment: biblioteca utilizada para a conversão de datas
