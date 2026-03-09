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

## Status do CI
Se você tiver um workflow criado, você pode adicionar um badge aqui.

Exemplo (substitua `WORKFLOW_FILE.yml` pelo nome do arquivo em `.github/workflows/`):
```markdown
![CI](https://github.com/IvanGabrielkg/ci-demo-uninassau/actions/workflows/WORKFLOW_FILE.yml/badge.svg)
```

## Como rodar o projeto localmente
> Ajuste os comandos conforme a linguagem do projeto.

### 1) Clonar o repositório
```bash
git clone https://github.com/IvanGabrielkg/ci-demo-uninassau.git
cd ci-demo-uninassau
```

### 2) Instalar dependências
**Exemplos:**

- Node.js:
```bash
npm install
```

- Python:
```bash
pip install -r requirements.txt
```

- Java (Maven):
```bash
mvn install
```

### 3) Rodar testes
**Exemplos:**
- Node.js:
```bash
npm test
```

- Python (pytest):
```bash
pytest -q
```

- Java (Maven):
```bash
mvn test
```

## Estrutura do repositório
> Preencha com a estrutura real do seu projeto.

Exemplo:
```text
.
├── .github/
│   └── workflows/
│       └── ci.yml
├── src/
├── tests/
└── README.md
```

## Boas práticas sugeridas
- Trabalhar com **branches** e abrir **Pull Requests**
- Não fazer merge com a pipeline quebrando
- Usar nomes e commits claros (ex.: Conventional Commits)
- Revisar PRs com checklist (testes, lint, documentação)

## Contribuição
Contribuições são bem-vindas!

1. Faça um fork do projeto
2. Crie uma branch: `git checkout -b feature/minha-feature`
3. Commit: `git commit -m "feat: minha feature"`
4. Push: `git push origin feature/minha-feature`
5. Abra um Pull Request

## Licença
Defina a licença do projeto (ex.: MIT).  
Se ainda não houver, você pode adicionar um arquivo `LICENSE`.

---
Feito para fins educacionais (demo de CI com GitHub Actions).
