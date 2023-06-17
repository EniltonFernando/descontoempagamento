# descontoempagamento
Elabore um algoritmo que calcule o que deve ser pago por um produto, considerando o preço normal de etiqueta (peça ao usuário) e a escolha da condição de pagamento. 

preco_etiqueta = float(input("Digite o preço normal de etiqueta: "))
condicao_pagamento = int(input("Digite a condição de pagamento (1, 2, 3 ou 4): "))

if condicao_pagamento == 1:
    valor_pagar = preco_etiqueta - (preco_etiqueta * 0.15)
elif condicao_pagamento == 2:
    valor_pagar = preco_etiqueta - (preco_etiqueta * 0.10)
elif condicao_pagamento == 3:
    valor_pagar = preco_etiqueta
elif condicao_pagamento == 4:
    valor_pagar = preco_etiqueta + (preco_etiqueta * 0.10)
else:
    print("Condição de pagamento inválida.")
    exit()

print("O valor a ser pago é: R$", valor_pagar)
