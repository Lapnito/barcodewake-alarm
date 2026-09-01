---
title: Missões e cadeias de missões do BarcodeWake
lang: pt
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# Missões e cadeias de missões do BarcodeWake

Uma missão do BarcodeWake é a condição usada para dispensar um alarme. A fonte atual suporta tarefas de código de barras, QR, matemática, digitação, agitar e passos, com NFC registrada tratada pelo caminho de varredura de código. As missões podem ser executadas sozinhas, em sequência ou por seleção aleatória.

## Missões de varredura criam distância física

Uma missão de código de barras ou QR compara uma varredura de câmera ao vivo com um código registrado durante a configuração. O código pode ser colocado em um objeto fora do alcance do braço: produtos de higiene no banheiro, um item do café da manhã na cozinha ou outro objeto estável em uma área bem iluminada. O NFC segue a mesma ideia geral com uma tag e um dispositivo compatível. O aplicativo armazena uma representação de hash nos caminhos atuais em vez de precisar do código bruto para comparação comum.

Escolha um objeto que ainda estará disponível quando o alarme tocar. As embalagens são descartadas, os rótulos desbotam e viagens mudam o ambiente. Registrar um código na única caixa de medicamento que você possa precisar trocar é menos robusto do que usar uma etiqueta durável. O [guia de configuração de alarme](../guides/set-up-an-alarm.md) aborda posicionamento e testes.

## Missões de desafio trocam movimento por esforço

Matemática e digitação exigem entrada focada. Agitar e passos exigem movimento físico e sensores compatíveis. As configurações de dificuldade e meta alteram a quantidade de trabalho esperada, mas uma missão mais difícil não é automaticamente melhor. Atrito excessivo pode incentivar desativar o alarme completamente, enquanto uma tarefa fácil pode se tornar automática após a repetição.

Combine a tarefa com o modo de falha. Se você desliga os alarmes sonolento, escanear em outro cômodo cria uma distância útil. Se o acesso à câmera for inconveniente, uma tarefa curta de digitação ou matemática pode ser mais prática. Se mobilidade, equilíbrio ou acessibilidade for uma preocupação, evite missões baseadas em movimento e escolha uma tarefa que possa ser concluída com segurança.

## Modos único, cadeia e aleatório

O modo único solicita uma missão configurada. O modo cadeia executa várias missões configuradas em ordem. O modo aleatório seleciona a partir de um conjunto configurado, reduzindo a chance de que uma interação memorizada se torne automática. Esses modos estão presentes na fonte mais recente verificada; a [disponibilidade](../availability.md) explica por que isso não prova que eles já estão em cada versão pública.

Sempre execute um teste a curto prazo após alterar o modo, permissões ou objetos registrados. Mantenha o objeto selecionado ao alcance e forneça uma rota de recuperação segura. Para problemas de entrega não relacionados à conclusão da missão, use a [lista de verificação de confiabilidade](../help/alarm-delivery.md).

