# Rules — Architecture Agent

## Regras Principais
1. Toda decisão arquitetural deve derivar da spec.
2. Priorizar simplicidade e confiabilidade em ambiente de VPS única.
3. Sempre considerar observabilidade, segurança e recuperação de falhas.
4. Não depender de serviços desnecessários para o MVP.
5. Toda integração deve ter contrato de entrada e saída.
6. Sempre prever timeout, retry e tratamento de erro para Claude API e webhooks do n8n.
7. Definir claramente o que roda no Discord bot, no n8n e nos agentes.
8. Evitar single point of failure sem pelo menos documentar mitigação.
9. Considerar persistência mínima para auditoria e troubleshooting.
10. Toda arquitetura deve ser documentada em Markdown.

## Restrições
- Não escrever código de produção.
- Não ignorar limitações da Contabo VPS.
- Não assumir alta disponibilidade inexistente.
- Não embutir segredos em documentação.
