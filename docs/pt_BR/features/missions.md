---
title: Missões e cadeias de missões do BarcodeWake
lang: pt_BR
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

Uma missão do BarcodeWake é a condição usada para dispensar um alarme. A fonte atual suporta tarefas de código de barras, QR, matemática, digitação, sacudir e passos, com NFC registrado tratado através do caminho de varredura de código. As missões podem ser executadas sozinhas, em sequência ou por seleção aleatória.

## Missões de varredura criam distância física

Uma missão de código de barras ou QR compara uma varredura de câmera ao vivo com um código registrado durante a configuração. O código pode ser colocado em um objeto fora do alcance do braço: itens de higiene no banheiro, um item de café da manhã na cozinha, ou outro objeto estável em uma área bem iluminada. NFC segue a mesma ideia geral com uma tag e dispositivo compatíveis. O aplicativo armazena uma representação de hash nos caminhos atuais em vez de necessitar do código bruto para comparação comum.

Escolha um objeto que ainda estará disponível quando o alarme tocar. A embalagem é descartada, os rótulos desbotam e a viagem muda o ambiente. Registrar um código na única caixa de medicamento que você pode precisar substituir é menos robusto do que usar um rótulo durável. O [guia de configuração de alarme](../guides/set-up-an-alarm.md) aborda posicionamento e testes.

## Missões de desafio trocam movimento por esforço

Matemática e digitação exigem entrada focada. Sacudir e passos exigem movimento físico e sensores suportados. As configurações de dificuldade e meta alteram quanto trabalho é esperado, mas uma missão mais difícil não é automaticamente uma melhor. Atrito excessivo pode encorajar desativar o alarme inteiramente, enquanto uma tarefa fácil pode se tornar automática após repetição.

Combine a tarefa ao modo de falha. Se você desliga alarmes sonolento, escanear em outro cômodo cria distância útil. Se o acesso à câmera é inconveniente, uma tarefa curta de digitação ou matemática pode ser mais prática. Se mobilidade, equilíbrio ou acessibilidade é uma preocupação, evite missões baseadas em movimento e escolha uma tarefa que possa ser completada com segurança.

## Modos único, cadeia e aleatório

Modo único pede uma missão configurada. Modo cadeia executa várias missões configuradas em ordem. Modo aleatório seleciona de um conjunto configurado, reduzindo a chance de que uma interação memorizada se torne automática. Esses modos estão presentes na fonte mais recente verificada; [disponibilidade](../availability.md) explica por que isso não prova que eles já estão em toda compilação pública.

Sempre execute um teste de curto prazo após alterar o modo, permissões ou objetos registrados. Mantenha o objeto selecionado ao alcance e forneça uma rota de recuperação segura. Para problemas de entrega não relacionados à conclusão da missão, use a [lista de verificação de confiabilidade](../help/alarm-delivery.md).

