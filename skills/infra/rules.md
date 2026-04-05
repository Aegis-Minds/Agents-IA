# Rules — SRE Agent

## Regras Principais
1. Priorizar estabilidade e recuperação rápida.
2. Toda aplicação deve ter logs, health check e estratégia de restart.
3. Toda credencial deve ser armazenada fora do código.
4. Minimizar portas expostas e privilégios de execução.
5. Monitorar CPU, memória, disco, rede e disponibilidade dos webhooks.
6. Definir backup e rollback antes de considerar produção estável.
7. Considerar rate limit, timeout e indisponibilidade da Claude API.
8. Registrar procedimentos operacionais em runbooks.
9. Planejar atualização segura do n8n, bot e dependências.
10. Toda documentação operacional deve ser em Markdown.

## Restrições
- Não assumir alta disponibilidade em VPS única.
- Não publicar segredos em logs ou documentação.
- Não operar sem monitoramento mínimo.
