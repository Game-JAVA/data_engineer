# Git


## O que é Git?

Git é um sistema de controle de versão distribuído amplamente utilizado para rastrear alterações em arquivos e coordenar o trabalho de várias pessoas em projetos de desenvolvimento de software. Criado por Linus Torvalds em 2005, Git permite que desenvolvedores colaborem de forma eficiente e segura.

### Principais Conceitos do Git

- **Repositório (Repo)**: Um diretório onde o Git armazena o histórico completo de mudanças do projeto, incluindo arquivos e pastas.
- **Commit**: Um snapshot do projeto em um ponto específico no tempo. Cada commit tem um identificador único (hash).
- **Branch**: Uma ramificação do projeto que permite trabalhar em diferentes linhas de desenvolvimento ao mesmo tempo. A branch principal é geralmente chamada de "main" ou "master".
- **Merge**: Combinação de mudanças de diferentes branches em uma única branch.
- **Pull**: Atualiza a cópia local do repositório com as mudanças mais recentes do repositório remoto.
- **Push**: Envia as mudanças locais para o repositório remoto.
- **Clone**: Criação de uma cópia local de um repositório remoto.
- **Fork**: Criação de uma cópia independente de um repositório, normalmente para contribuir com um projeto sem afetar o repositório original.

### Benefícios do Git

- **Controle de Versão**: Mantém o histórico completo de mudanças, permitindo reverter para versões anteriores se necessário.
- **Colaboração**: Facilita o trabalho em equipe, permitindo que múltiplos desenvolvedores trabalhem simultaneamente em diferentes partes do projeto.
- **Distribuído**: Cada desenvolvedor tem uma cópia completa do repositório, aumentando a resiliência e a flexibilidade.

Cursos e artigos úteis:

[Introdução ao GIT](https://www.udemy.com/course/git-e-github-para-iniciantes/learn/lecture/5120538?start=0#overview)

### Introdução ao GitFlow

GitFlow é um modelo de branching (ramificação) para o uso do Git assim com github flow, ele estabelece um conjunto de procedimentos para gerenciar branches de forma organizada e eficiente, especialmente em projetos de software colaborativos e de larga escala.

![Untitled](images/gitflow.png)

### Principais Componentes do GitFlow

1. **Branches Principais**:
    - **main**: Contém o código de produção estável. Cada commit nesta branch representa uma nova versão de lançamento.
    - **develop**: Contém o código em desenvolvimento com as últimas alterações aprovadas. Serve como a base para novas funcionalidades e integrações.
2. **Branches de Suporte**:
    - **feature**: Usada para desenvolver novas funcionalidades. Deriva de `develop` e é mesclada de volta a `develop` quando a funcionalidade está concluída.
    - **release**: Preparada para o lançamento de uma nova versão. Deriva de `develop` e, após ajustes finais, é mesclada em `main` e `develop`.
    - **hotfix**: Criada para correções urgentes em produção. Deriva de `main` e é mesclada de volta em `main` e `develop` após a correção.

### Fluxo de Trabalho

1. **Desenvolvimento de Funcionalidades**:
    - Crie uma branch de `feature` a partir de `develop`.
    - Desenvolva a nova funcionalidade.
    - Mescle a branch de `feature` de volta em `develop`.
2. **Preparação para Lançamento**:
    - Crie uma branch de `release` a partir de `develop`.
    - Faça os ajustes finais e correções.
    - Mescle a branch de `release` em `main` e `develop`, e marque o commit com um tag.
3. **Correções Urgentes**:
    - Crie uma branch de `hotfix` a partir de `main`.
    - Faça a correção necessária.
    - Mescle a branch de `hotfix` em `main` e `develop`, e marque o commit com um tag.

### Benefícios do GitFlow

- **Organização**: Estrutura clara para gerenciar diferentes tipos de trabalho.
- **Paralelismo**: Facilita o trabalho simultâneo em múltiplas funcionalidades e correções.
- **Estabilidade**: Garante que o código em produção está sempre em estado estável.

GitFlow é um modelo eficaz para manter a organização e a qualidade no desenvolvimento de software, especialmente em equipes que trabalham em projetos complexos e colaborativos.

Cursos e artigos úteis:

- [Gitflow conceito](https://www.alura.com.br/artigos/git-flow-o-que-e-como-quando-utilizar)
- [Gitflow cheatsheet](https://danielkummer.github.io/git-flow-cheatsheet/)
- [Gitflow extension](https://github.com/nvie/gitflow)