# Algoritmo – Controle de Acesso de Alunos em Sala

Estudante: Geovana Silveira Endres

RGM: 38193248

# Objetivo

Organizar o processo de entrada dos alunos na sala de aula de forma lógica e sistemática, verificando se cada aluno está presente na lista oficial da turma.

# Pseudocódigo

    INÍCIO

    Exibir mensagem:
    "Sistema de Controle de Acesso iniciado"

    Enquanto houver alunos na fila faça

    Ler nome do aluno

    Exibir mensagem:
    "Verificando acesso do aluno..."

    SE nome do aluno estiver na lista oficial ENTÃO

        Exibir mensagem:
        "Aluno encontrado na lista"

        Exibir mensagem:
        "Entrada permitida"

        Registrar presença do aluno

    SENÃO

        Exibir mensagem:
        "ERRO: aluno não encontrado na lista oficial"

        Exibir mensagem:
        "Entrada negada"

        Encaminhar aluno para verificação manual

    FIM SE

    Exibir mensagem:
    "Próximo aluno da fila"

    FIM ENQUANTO

    Exibir mensagem:
    "Todos os alunos foram verificados"

    FIM


# Explicação da Lógica Utilizada

O algoritmo foi desenvolvido utilizando estruturas de decisão e repetição para organizar o controle de entrada dos alunos.

# Estrutura de Repetição

Foi utilizado o comando “Enquanto” para garantir que todos os alunos presentes na fila fossem verificados individualmente.

# Estrutura Condicional

Foi utilizada a estrutura “Se-Então-Senão” para decidir se o aluno teria acesso permitido ou negado.

- Se o nome estiver na lista oficial:
    - a entrada é autorizada;
    - a presença é registrada.

- Caso contrário:
    - o sistema exibe uma mensagem de erro;
    - a entrada é bloqueada;
    - o aluno é encaminhado para conferência manual.

# Aplicação do Pensamento Computacional

O algoritmo utiliza conceitos do pensamento computacional, como:

- Decomposição:
divisão do problema em etapas menores.

- Abstração:
foco apenas nas informações necessárias para o controle de acesso.

- Algoritmo:
criação de uma sequência lógica de instruções para resolver o problema.

# Conclusão

A atividade demonstrou como o pensamento lógico e algorítmico pode ser aplicado em situações do cotidiano. A utilização de estruturas condicionais e de repetição permitiu criar um processo organizado, eficiente e de fácil execução para o controle de acesso dos alunos.
