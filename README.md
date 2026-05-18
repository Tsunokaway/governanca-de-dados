---
 
## 📌 Contexto
 
A EduTech Forward enfrenta quatro problemas centrais de governança:
 
- 📂 **Dados descentralizados** — cada área usa sistemas e nomenclaturas próprias
- ❌ **Cancelamentos sem rastreabilidade** — acesso do aluno permanece ativo por até 48h
- 🧠 **Perda de memória técnica** — decisões arquiteturais se perdem com a rotatividade
- 📖 **Sem dicionário de dados** — termos como "aluno ativo" têm definições conflitantes
---
 
## 📁 Estrutura do Repositório
 
```
governanca-de-dados_EDTECH-FORWARD/
│
├── 📂 processos/
│   └── README.md
│
├── 📂 dicionario-de-dados/
│   └── README.md
│
├── 📂 governanca/
│   ├── README.md
│   └── README.md
│
├── 📂 arquitetura/
│   ├── decisoes/
│   └── README.md
│
└── README.md
```
 
---
 
## 📦 Entregáveis
 
| # | Entregável | Responsável | Status |
|---|-----------|-------------|--------|
| 1 | Mapa de Atores e Responsabilidades | — | 🔄 Em andamento |
| 2 | Dicionário de Dados | — | 🔄 Em andamento |
| 3 | Estrutura do Repositório (este repo) | — | 🔄 Em andamento |
| 4 | Padrão de Nomenclatura de Tabelas | — | 🔄 Em andamento |
| 5 | Análise de Riscos e LGPD | — | 🔄 Em andamento |
 
---
 
## 🔐 Controle de Acesso
 
| Pasta | Permissão de Escrita | Permissão de Leitura |
|-------|---------------------|---------------------|
| `processos/` | Time de Processos | Todos |
| `dicionario-de-dados/` | Time de Dados | Todos |
| `governanca/` | Data Owner | Todos |
| `arquitetura/` | Time Técnico | Todos |
 
---
 
## 🌿 Fluxo de Contribuição
 
Nenhuma alteração deve ser feita diretamente na branch `main`.
 
```bash
# 1. Crie um branch para sua alteração
git checkout -b doc/nome-da-alteracao
 
# 2. Faça as alterações e commite
git add .
git commit -m "docs: descrição clara da alteração"
 
# 3. Envie para o GitHub
git push origin doc/nome-da-alteracao
 
# 4. Abra um Pull Request para revisão
```
 
> ⚠️ A branch `main` possui **branch protection** ativada — todo merge requer aprovação de ao menos 1 revisor.
 
---

 
## 📚 Referências
 
- Slides — Data Ethics, Governance & Security in the AI Age
- [Lei Geral de Proteção de Dados — LGPD (Lei nº 13.709/2018)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)
- [GitHub Docs — Branch Protection Rules](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches)
---
 
<div align="center">
  <sub>Checkpoint 3 · Data Ethics, Governance & Security in the AI Age · DataVault Soluções</sub>
</div>
