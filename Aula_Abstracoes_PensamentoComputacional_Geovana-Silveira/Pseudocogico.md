# Algoritmo Pedido De Comida

INÍCIO

    // Verificar conexão com internet
    SE internet_disponivel = FALSO ENTÃO
        EXIBIR "Sem conexão com a internet."
        ENCERRAR
    FIMSE

    // Abrir aplicativo
    ABRIR aplicativo_delivery

    // Realizar login
    FAZER login

    SE login_valido = FALSO ENTÃO
        EXIBIR "Erro ao realizar login."
        ENCERRAR
    FIMSE

    // Buscar restaurantes
    LISTAR restaurantes_disponiveis

    // Selecionar restaurante
    restaurante ← ESCOLHER restaurante

    // Visualizar cardápio
    MOSTRAR cardapio(restaurante)

    // Inicializar carrinho
    carrinho ← vazio

    REPITA

        // Selecionar produto
        produto ← ESCOLHER produto

        // Selecionar quantidade
        quantidade ← INFORMAR quantidade

        // Adicionar ao carrinho
        ADICIONAR produto, quantidade AO carrinho

        // Perguntar se deseja continuar
        EXIBIR "Deseja adicionar mais itens?"
        resposta ← LER resposta

    ATÉ resposta = "não"

    // Verificar carrinho
    SE carrinho = vazio ENTÃO
        EXIBIR "Carrinho vazio."
        ENCERRAR
    FIMSE

    // Exibir resumo do pedido
    MOSTRAR resumo(carrinho)

    // Escolher forma de pagamento
    pagamento ← ESCOLHER forma_pagamento

    // Validar pagamento
    SE pagamento_aprovado = FALSO ENTÃO
        EXIBIR "Pagamento recusado."
        ENCERRAR
    FIMSE

    // Confirmar pedido
    CONFIRMAR pedido

    // Enviar pedido ao restaurante
    ENVIAR pedido

    // Verificar aceite do restaurante
    SE restaurante_aceitou = FALSO ENTÃO
        EXIBIR "Pedido cancelado pelo restaurante."
        ENCERRAR
    FIMSE

    // Acompanhar entrega
    ENQUANTO pedido_entregue = FALSO FAÇA
        MOSTRAR status_entrega
    FIMENQUANTO

    // Finalização
    EXIBIR "Pedido entregue com sucesso."

    // Avaliação
    avaliacao ← INFORMAR nota_avaliacao

    SALVAR avaliacao

FIM
