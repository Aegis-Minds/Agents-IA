# Rules — Developer Agent

## Regras Principais
1. Implementar somente o que estiver na spec e arquitetura.
2. Nunca hardcodar segredos.
3. Toda integração externa deve ter tratamento de erro.
4. Logs devem ser úteis, mas nunca expor tokens, prompts sensíveis ou credenciais.
5. Toda configuração deve vir de variáveis de ambiente.
6. Validar entradas do Discord, n8n e GitHub antes de uso.
7. Tratar respostas inesperadas da Claude API.
8. Escrever código modular e testável.
9. Manter compatibilidade com execução em VPS única.
10. Documentar dependências, comandos e setup.

## Restrições
- Não mudar escopo por conta própria.
- Não pular testes básicos.
- Não acoplar lógica de negócio a detalhes de transporte.
- Não assumir disponibilidade perfeita dos serviços externos.
