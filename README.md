# Agents IA

Estrutura pronta para repositório dos agentes do projeto **Agents-IA**.

## Contexto
- Entrada de comandos e acionamentos via Discord
- Orquestração e automações via n8n
- Infraestrutura em VPS Contabo
- Processamento de IA via API da Claude
- Pipeline de agentes: Spec → Architecture → Developer → QA → SRE
- Referência de rastreabilidade: GitHub Issue #2

## Estrutura
```text
agents/
  spec/
    skill.md
    rules.md
  architecture/
    skill.md
    rules.md
  developer/
    skill.md
    rules.md
  qa/
    skill.md
    rules.md
  sre/
    skill.md
    rules.md
```

## Uso sugerido
- `skill.md` define o papel, responsabilidades, entradas, saídas e boas práticas do agente.
- `rules.md` define regras operacionais, restrições e critérios obrigatórios.
- Cada agente deve consumir a saída do anterior sempre que aplicável.

## Fluxo sugerido
1. **Spec** transforma issue e contexto em especificação objetiva.
2. **Architecture** converte a spec em desenho técnico e contratos.
3. **Developer** implementa conforme spec e arquitetura.
4. **QA** valida critérios de aceite, integração e regressão.
5. **SRE** garante deploy, observabilidade, segurança e operação.

## Integrações principais
- Discord
- n8n
- Claude API
- GitHub
- VPS Contabo

## Observações
- Os arquivos estão em Markdown e prontos para commit.
- A estrutura foi pensada para funcionar bem com orquestração por agentes e repositórios monolíticos simples.
