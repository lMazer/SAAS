# Como adicionar um novo projeto à capa

Use este checklist sempre que um produto SaaS ou projeto documental entrar no índice público. Identifique com clareza se está implantado, em evolução ou em planejamento.

## 1. Dados mínimos

Preencha e adicione uma linha na tabela **Resumo** do [README.md](../README.md):

| Campo | Exemplo |
|-------|---------|
| Projeto | Nome comercial |
| Stack | 3–5 tecnologias principais |
| Status | Produção / Em evolução / Em planejamento |
| Última alteração | Data da última atualização documental ou entrega relevante (`DD/MM/AAAA`) |
| Site | URL pública https ou `Ainda não disponível` |

## 2. Bloco de case

No README, crie uma seção `### Nome do Projeto` com:

1. Screenshot em `docs/previews/nome-do-projeto.png`, quando houver interface disponível
2. Uma frase sobre o problema/entrega
3. Bullet **Stack**
4. Bullet **Entrega**
5. Bullet **Destaques técnicos** (até 3)
6. Bullet **Repositório** (`lMazer/...` — privado, se aplicável)
7. Bullet **Site** (link clicável ou `Ainda não disponível`)

Para projetos documentais ou em planejamento sem interface/site público, não invente capturas nem URLs. Explique o estágio atual e descreva a entrega documental sem sugerir que exista produto implantado.

## 3. Screenshot

- Quando houver interface, capturar a home/app em desktop (viewport largo)
- Salvar PNG em `docs/previews/`
- Referenciar no README com caminho relativo

## 4. Commit

Sugestão de mensagem:

```text
docs: adiciona [Nome do Projeto] ao índice de SaaS
```

## Modelo rápido (copiar/colar)

```markdown
### Nome do Projeto

<!-- Inclua a imagem quando houver interface pública ou captura autorizada. -->

Uma frase sobre a entrega.

- **Stack:** ...
- **Entrega:** ...
- **Destaques técnicos:** ...
- **Repositório:** `lMazer/exemplo-saas` *(privado)*
- **Site:** [exemplo.com.br](https://exemplo.com.br) ou `Ainda não disponível`
```
