# ci-demo-uninassau
Continuous Integration (CI) - Configurando pipelines com GitHub Actions

## Sobre o projeto
Este repositório é uma **demonstração prática** de como configurar **pipelines de Integração Contínua (CI)** usando **GitHub Actions**.

A proposta é servir como material de apoio (aulas/labs) para:
- entender os conceitos de CI;
- automatizar validações a cada push/pull request;
- rodar testes e checagens de qualidade;
- evitar regressões antes de fazer merge.

## Objetivos
- Configurar um workflow de CI do zero
- Executar o pipeline automaticamente em eventos (push/PR)
- Padronizar a qualidade do código com verificações automáticas
- (Opcional) Publicar artefatos / relatórios (ex.: coverage, lint)

## Tecnologias
- GitHub Actions (workflows)
- Git/GitHub (versionamento e PRs)
- [adicione aqui a stack do projeto: Node.js, Java, Python etc.]

## Como funciona a pipeline (CI)
Os workflows ficam em:
- `.github/workflows/`

Em geral, a pipeline pode conter etapas como:
1. Checkout do código
2. Configuração do ambiente (ex.: Node/Java/Python)
3. Instalação de dependências
4. Lint / formatação (opcional)
5. Testes automatizados
6. Build (se aplicável)

> Observação: adapte esta seção de acordo com o(s) workflow(s) real(is) do repositório.
Estrutura do projeto
- `.github/workflows/ci.yml`
- `README.md`

## Explicação do workflow (`ci.yml`)
- `name: CI Test`  
  Define o nome do workflow que aparece na aba **Actions** do GitHub.
- `on: [push]`  
  Configura o gatilho: o workflow executa sempre que houver **push** no repositório.
- `jobs:`  
  Define os “trabalhos” (jobs) do workflow.
- `test:`  
  Nome do job (pode ser qualquer nome).
- `runs-on: ubuntu-latest`  
  Define o ambiente de execuç��o (runner) como uma VM Linux Ubuntu.
- `steps:`  
  Lista de etapas executadas em sequência dentro do job.
  - `Mensagem 1` → `run: echo "Iniciando pipeline"`  
    Exibe a primeira mensagem no log.
  - `Mensagem 2` → `run: echo "Pipeline finalizado"`  
    Exibe a segunda mensagem no log.

## Fluxo do pipeline
Push no GitHub  
↓  
GitHub Actions inicia o workflow (`CI Test`)  
↓  
Job `test` roda no `ubuntu-latest`  
↓  
Execução dos `steps` (echo das mensagens)  
↓  
Resultado aparece nos logs do Actions

## Resultado da execução
Quando o pipeline é executado, o GitHub Actions cria uma execução do workflow e, nos logs, aparecem as mensagens:
- `Iniciando pipeline`
- `Pipeline finalizado`
---
Feito para fins educacionais (demo de CI com GitHub Actions).
