# SAAS

Índice público de produtos SaaS.

Este repositório é uma **capa de portfólio**: documenta o que foi entregue, a stack e os produtos ao vivo. O código de cada projeto fica em repositórios **privados** (clientes / NDA).

## Resumo

| Projeto | Stack | Status | Última alteração | Site |
|---------|-------|--------|------------------|------|
| Efathá Hosting Manager | Spring Boot, React/TypeScript, PostgreSQL, Docker, Traefik | Baseline / Em evolução | 22/09/2026 | — |

## Cases

### Efathá Hosting Manager

Painel SaaS para centralizar clientes, projetos hospedados, status público (ativo / manutenção / bloqueado / desativado), cobranças e notificações — sem substituir cPanel/Plesk, com bloqueio preferencial via roteamento no Traefik.

- **Stack:** Spring Boot (monólito modular), React + TypeScript, PostgreSQL, Docker, Traefik; integrações (Efí, Resend) atrás de ports
- **Entrega:** baseline documental completa (BMAP, PRD, SDD, TDD, BDD, modelo de dados, ADRs); implementação de código ainda em preparação
- **Destaques técnicos:** um estado operacional por projeto; página pública neutra em `BLOQUEADO`; agente de VPS com privilégios mínimos (evolução planejada)
- **Repositório:** `lMazer/efatha-hosting-manager` *(privado)*
- **Site:** — *(ainda sem URL pública)*

Projetos adicionais seguirão o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).

## Padrões que sigo

- Layout responsivo (mobile → desktop)
- SEO básico (títulos, meta, sitemap/robots quando aplicável)
- Performance de assets (imagens otimizadas, peso consciente)
- Acessibilidade mínima (semântica HTML, contraste, navegação por teclado onde faz sentido)
- Documentação e caminho de deploy claros em cada projeto

## Como adicionar um novo projeto

Siga o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).
