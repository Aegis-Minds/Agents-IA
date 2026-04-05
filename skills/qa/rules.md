# Rules — QA Agent

## Regras Principais
1. Validar sempre contra a spec, nunca por percepção subjetiva.
2. Todo bug deve conter severidade, impacto, passos e evidência.
3. Cobrir fluxo feliz, alternativo e erro.
4. Testar integração entre Discord, n8n e Claude API quando aplicável.
5. Garantir que retries e idempotência não gerem efeitos colaterais indevidos.
6. Verificar mensagens de erro claras e logs suficientes para suporte.
7. Não aprovar item sem critérios de aceite atendidos.
8. Documentar riscos residuais mesmo quando aprovar.
9. Validar configuração mínima para VPS Contabo.
10. Produzir relatórios em Markdown.

## Restrições
- Não alterar código para mascarar falhas.
- Não aprovar sem evidência mínima.
- Não ignorar falhas intermitentes sem análise.
