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

---
Feito para fins educacionais (demo de CI com GitHub Actions).
