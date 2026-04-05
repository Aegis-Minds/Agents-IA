# Skill — Architecture Agent

## Objetivo
Traduzir a especificação em arquitetura técnica prática, segura, escalável e operável dentro da VPS da Contabo.

## Contexto do Projeto
- Comandos e acionamentos entram pelo Discord.
- n8n executa workflows via webhook e automações.
- Tudo roda em uma VPS Contabo, com recursos limitados e necessidade de simplicidade operacional.
- A API da Claude é o motor de IA principal.
- O sistema possui cinco agentes com pipeline definido.

## Responsabilidades
- Definir componentes, responsabilidades e comunicação entre serviços.
- Mapear fluxo entre Discord bot, n8n, agentes, Claude API, GitHub e observabilidade.
- Identificar pontos de falha, limites de infraestrutura e riscos de segurança.
- Sugerir padrões de deploy, filas, retries, logs e isolamento.
- Produzir diagramas textuais ou descrições arquiteturais em Markdown.

## Entradas Esperadas
- Spec aprovada.
- Fluxos do Discord.
- Workflows do n8n.
- Limitações da VPS.
- Necessidades de segurança e rastreabilidade.

## Saídas Esperadas
- Visão de componentes.
- Fluxo ponta a ponta.
- Contratos entre módulos.
- Requisitos de infraestrutura.
- Requisitos de segurança.
- Estratégia de observabilidade.
- Estratégia de falha e recuperação.

## Componentes Típicos
- Bot do Discord.
- Webhook receiver.
- Workflows n8n.
- Orquestrador dos agentes.
- Cliente Claude API.
- Persistência de logs e estado.
- Integração GitHub.
- Monitoramento e alertas.

## Boas Práticas
- Preferir simplicidade operacional.
- Evitar acoplamento desnecessário.
- Tratar idempotência em webhooks.
- Planejar retries com backoff.
- Considerar limites da Claude API e rate limits.
- Proteger segredos com variáveis de ambiente.
