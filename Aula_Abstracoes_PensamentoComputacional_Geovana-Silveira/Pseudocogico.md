# Nível 3 — Abstração Computacional (Pseudocódigo)

```plaintext
ALGORITMO Sistema_Pedido_Delivery

INÍCIO

    // Verificação de conexão
    SE internet_disponivel = FALSO ENTÃO
        EXIBIR "Erro: conexão com a internet indisponível."
        ENCERRAR_ALGORITMO
    FIMSE


    // Inicialização do sistema
    ABRIR aplicativo_delivery

    REALIZAR login_usuario


    // Validação de acesso
    SE login_valido = FALSO ENTÃO
        EXIBIR "Erro ao autenticar usuário."
        ENCERRAR_ALGORITMO
    FIMSE


    // Consulta de restaurantes
    LISTAR restaurantes_disponiveis

    restaurante_selecionado ← ESCOLHER restaurante


    // Exibição do cardápio
    MOSTRAR cardapio(restaurante_selecionado)


    // Inicialização do carrinho
    carrinho ← VAZIO


    // Processo de seleção de produtos
    REPITA

        produto ← ESCOLHER item_cardapio

        quantidade ← INFORMAR quantidade_desejada

        ADICIONAR produto, quantidade AO carrinho

        EXIBIR "Deseja adicionar mais itens ao pedido?"
        resposta ← LER resposta_usuario

    ATÉ resposta = "NÃO"


    // Validação do carrinho
    SE carrinho = VAZIO ENTÃO
        EXIBIR "Nenhum item selecionado."
        ENCERRAR_ALGORITMO
    FIMSE


    // Resumo do pedido
    MOSTRAR resumo_pedido(carrinho)


    // Seleção de pagamento
    metodo_pagamento ← ESCOLHER forma_pagamento


    // Validação financeira
    SE pagamento_aprovado = FALSO ENTÃO
        EXIBIR "Pagamento não autorizado."
        ENCERRAR_ALGORITMO
    FIMSE


    // Confirmação do pedido
    CONFIRMAR pedido


    // Envio ao restaurante
    ENVIAR pedido_para_restaurante


    // Retorno do restaurante
    SE restaurante_aceitou = FALSO ENTÃO
        EXIBIR "Pedido recusado pelo restaurante."
        CANCELAR pedido
        ENCERRAR_ALGORITMO
    FIMSE


    // Acompanhamento da entrega
    ENQUANTO pedido_entregue = FALSO FAÇA

        MOSTRAR status_entrega

    FIMENQUANTO


    // Finalização
    EXIBIR "Pedido entregue com sucesso."


    // Avaliação do usuário
    nota_avaliacao ← INFORMAR nota

    SALVAR avaliacao_usuario


FIM
```

