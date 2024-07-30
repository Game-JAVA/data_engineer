# Linux/Shell


### Introdução ao Shell Script

**Shell Script** é um tipo de script de computador que é executado por um shell Unix ou Linux. Shell scripts são arquivos de texto que contêm uma série de comandos que o shell pode interpretar e executar. Eles são usados para automatizar tarefas repetitivas e simplificar a execução de comandos complexos no ambiente de linha de comando.

### Conceitos Principais

1. **Shell**: O shell é um programa que fornece uma interface de linha de comando para interagir com o sistema operacional. Exemplos de shells incluem Bash (Bourne Again Shell), Zsh (Z Shell) e Sh (Bourne Shell).
2. **Script**: Um script é um arquivo que contém uma sequência de comandos que são executados pelo shell. Ele pode incluir variáveis, loops, condicionais e funções para executar tarefas automatizadas.
3. **Comandos**: Shell scripts consistem em comandos que o shell pode executar, como `ls` para listar arquivos, `grep` para buscar padrões, e `cp` para copiar arquivos.
4. **Variáveis**: Variáveis em shell scripts são usadas para armazenar dados que podem ser utilizados em comandos e operações. Elas são definidas com um nome e podem armazenar valores como strings ou números.
5. **Loops e Condicionais**: Shell scripts podem incluir estruturas de controle, como loops (`for`, `while`) e condicionais (`if`, `else`), para executar comandos repetidamente ou tomar decisões com base em condições.
6. **Funções**: Funções permitem encapsular um conjunto de comandos em um bloco reutilizável, facilitando a modularização e a manutenção do script.

### Importância do Aprendizado de Shell Script

1. **Automatização de Tarefas Repetitivas**: Shell scripts permitem a automação de tarefas repetitivas, como backups, instalação de software e monitoramento de sistemas. Isso economiza tempo e reduz erros ao eliminar a necessidade de executar comandos manualmente.
2. **Eficiência e Produtividade**: Ao automatizar processos, os shell scripts aumentam a eficiência e a produtividade, permitindo que você execute operações complexas com um único comando.
3. **Administração de Sistemas**: Shell scripts são essenciais para a administração e configuração de sistemas Unix e Linux. Eles permitem a criação de scripts de inicialização, gerenciamento de usuários, e configuração de redes.
4. **Desenvolvimento e Testes**: Em ambientes de desenvolvimento, shell scripts são usados para compilar código, executar testes e gerenciar ambientes de desenvolvimento. Eles facilitam a integração contínua e o deploy de software.
5. **Flexibilidade e Controle**: Shell scripts oferecem um alto grau de flexibilidade e controle sobre o ambiente de sistema e as tarefas de administração. Eles podem ser usados para personalizar o comportamento do sistema e criar soluções sob medida para problemas específicos.
6. **Facilidade de Aprendizado**: Shell scripting é relativamente fácil de aprender e usar, especialmente para quem já está familiarizado com o ambiente de linha de comando. É uma habilidade prática que pode ser aplicada rapidamente para resolver problemas e automatizar tarefas.

### Exemplos Simples de Shell Script

1. **Script de Backup**:
    
    ```bash
    bashCopiar código
    #!/bin/bash
    tar -czf /backup/meuarquivo_backup_$(date +%F).tar.gz /meuarquivo
    
    ```
    
2. **Script de Verificação de Espaço em Disco**:
    
    ```bash
    bashCopiar código
    #!/bin/bash
    echo "Espaço disponível em disco:"
    df -h
    
    ```
    
3. **Script de Monitoramento de Processos**:
    
    ```bash
    bashCopiar código
    #!/bin/bash
    if pgrep "processo_exemplo" > /dev/null
    then
        echo "O processo está em execução."
    else
        echo "O processo não está em execução."
    fi
    
    ```
    

### Conclusão

Aprender shell scripting é uma habilidade fundamental para administradores de sistemas, desenvolvedores e qualquer pessoa que trabalhe com sistemas Unix ou Linux. Ele oferece uma maneira poderosa de automatizar tarefas, aumentar a eficiência e ter um controle mais preciso sobre o ambiente de sistema. Com o shell scripting, você pode simplificar processos complexos, criar soluções personalizadas e melhorar a produtividade geral.

Saiba mais:

[Bash comands](https://developers.redhat.com/cheat-sheets/bash-shell-cheat-sheet)

[Curso shell script](https://www.udemy.com/course/draft/1908478/learn/lecture/11750810?start=0#overview)