# Resumo de Como os Problemas Foram Evitados

## Deadlock

- **Limitamos o número de filósofos** que podem tentar comer ao mesmo tempo usando um **semáforo**.
- **Quebramos a simetria** invertendo a ordem de pegar os garfos para filósofos na fila de prioridade.

## Starvation

- **Implementamdo uma fila de prioridade** para filósofos que estão esperando há muito tempo.
- **É monitorado o tempo** que cada filósofo fica sem comer e garantimos que todos tenham a chance de comer.
- Caso aconteça um caso de starvation(Não ocorreu nas simulações) o processo é reiniciado.

## Race Condition

- **Utilizado locks** para sincronizar o acesso a recursos compartilhados, como garfos e a fila de prioridade.
- **Garantimos que apenas uma thread** possa acessar um recurso crítico de cada vez.



Exemplo do código em funcionamento.
