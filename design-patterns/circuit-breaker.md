# CIRCUIT BREAKER

Criado por Michael Nygard e lançado em seu livro.

- design pattern para apis.
- evitar requests denecessários quando algum serviço estiver fora.
- request handler - ( http manager pode desempenhar esse papel? )

request handler status
- ALLOW ......... CLOSED
- STOP .......... OPEN
- ALLOW PARTIAL . HALF OPEN

