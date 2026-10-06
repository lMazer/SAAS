# SAAS

Índice público de produtos SaaS.

Este repositório é uma **capa de portfólio**: documenta produtos em evolução e projetos SaaS em planejamento, com seu estágio, stack e disponibilidade pública. O código e a documentação de cada projeto ficam em repositórios **privados**.

## Resumo

| Projeto | Stack | Status | Última alteração | Site |
|---------|-------|--------|------------------|------|
| Efathá Hosting Manager | Java/Quarkus 3, React/TypeScript, Keycloak, PostgreSQL, Docker, Traefik | Em evolução | 06/10/2026 | [gestao.efathasolutions.com.br](https://gestao.efathasolutions.com.br) |
| Efathá Avdá | Java 25/Quarkus, React/TypeScript, Expo/React Native, Keycloak, PostgreSQL | Em planejamento | 06/10/2026 | Ainda não disponível |

## Cases

### Efathá Hosting Manager

![Login Efathá Hosting Manager](docs/previews/efatha-hosting-manager.png)

SaaS para gestão operacional e financeira de sites, landing pages e projetos hospedados — painel interno Efathá e portal do cliente (faturas, Pix, histórico), com bloqueio preferencial via roteamento no Traefik (sem substituir cPanel/Plesk).

- **Stack:** Java / Quarkus 3 (monólito modular), React + TypeScript, PostgreSQL, Keycloak (OIDC) + BFF, Docker + Traefik; integrações de cobrança/notificação atrás de ports
- **Entrega:** documentação de produto e arquitetura; implementação em evolução, incluindo RBAC, dashboard e gestão de usuários/perfis; painel em `gestao.efathasolutions.com.br`. Estado documental consultado em 06/10/2026.
- **Destaques técnicos:** um estado operacional por projeto; página pública neutra em `BLOQUEADO`; papéis dinâmicos no banco (em vez de enum fixo); agente de VPS com privilégios mínimos (evolução planejada)
- **Repositório:** `lMazer/efatha-hosting-manager` *(privado)*
- **Site:** [https://gestao.efathasolutions.com.br](https://gestao.efathasolutions.com.br)

#### Galeria do Hosting Manager

Capturas do painel Efathá Hosting Manager (ambiente de teste / admin local).

| Login | Dashboard | Clientes |
|:---:|:---:|:---:|
| ![Login](docs/previews/efatha-hosting-manager.png) | ![Dashboard](docs/previews/efatha-dashboard.png) | ![Clientes](docs/previews/efatha-clientes.png) |
| **Contratos** | **Serviços** | **Contas a pagar** |
| ![Contratos](docs/previews/efatha-contratos.png) | ![Serviços](docs/previews/efatha-servicos.png) | ![Contas a pagar](docs/previews/efatha-contas-pagar.png) |
| **Contas a receber** | **Projetos** | **Servidores** |
| ![Contas a receber](docs/previews/efatha-contas-receber.png) | ![Projetos](docs/previews/efatha-projetos.png) | ![Servidores](docs/previews/efatha-servidores.png) |
| **Usuários** | **Perfis (ACL)** | **Política comercial** |
| ![Usuários](docs/previews/efatha-config-acesso.png) | ![Perfis](docs/previews/efatha-config-perfis.png) | ![Comercial](docs/previews/efatha-config-comercial.png) |
| **Aparência (login)** | **Sessões** | |
| ![Aparência](docs/previews/efatha-config-aparencia.png) | ![Sessões](docs/previews/efatha-sessoes.png) | |

### Efathá Avdá

Projeto SaaS multi-tenant para gestão de voluntários, ministérios, eventos, escalas, check-in, comunicação e operação de igrejas.

- **Stack aprovada:** Java 25 / Quarkus (monólito modular), React 19.2, TypeScript 6, Vite 8, Expo SDK 57 / React Native 0.86, Keycloak e PostgreSQL 18.
- **Entrega:** especificação e governança do produto; arquitetura aprovada pela ADR-013 em 06/10/2026. O projeto está em planejamento e sua documentação permanece em revisão final; não representa produto implantado.
- **Destaques técnicos:** multi-tenancy com `tenant_id` e RLS; PostgreSQL compartilhado por ambiente; Traefik existente como edge.
- **Repositório:** `lMazer/efatha-avda` *(privado; repositório de especificação e governança)*
- **Site:** ainda não disponível.

Novos projetos seguirão o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md), que também cobre cases em planejamento sem site ou interface pública.

## Padrões que sigo

- Layout responsivo (mobile → desktop)
- SEO básico (títulos, meta, sitemap/robots quando aplicável)
- Performance de assets (imagens otimizadas, peso consciente)
- Acessibilidade mínima (semântica HTML, contraste, navegação por teclado onde faz sentido)
- Documentação e caminho de deploy claros em cada projeto

## Como adicionar um novo projeto

Siga o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).
