---
title: Missões e cadeias de missões do BarcodeWake
lang: pt_PT
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

Uma missão do BarcodeWake é a condição utilizada para dispensar um alarme. A fonte atual suporta tarefas de código de barras, QR, matemática, digitação, agitação e passos, com NFC registado tratado através do caminho de digitalização de código. As missões podem ser executadas individualmente, em sequência ou por seleção aleatória.

## Missões de digitalização criam distância física

Uma missão de código de barras ou QR compara uma digitalização de câmara em direto com um código registado durante a configuração. O código pode ser colocado num objeto fora do alcance do braço: produtos de higiene numa casa de banho, um item do pequeno-almoço numa cozinha, ou outro objeto estável numa área bem iluminada. O NFC segue a mesma ideia geral com uma etiqueta compatível e dispositivo. A aplicação armazena uma representação hash nos caminhos atuais em vez de necessitar do código cru para comparação ordinária.

Escolha um objeto que ainda estará disponível quando o alarme tocar. As embalagens são descartadas, as etiquetas desvanecem-se e as viagens alteram o ambiente. Registar um código na única caixa de medicamentos que pode necessitar de substituir é menos robusto do que usar uma etiqueta durável. O [guia de configuração de alarme](../guides/set-up-an-alarm.md) aborda a colocação e os testes.

## Missões de desafio trocam movimento por esforço

A matemática e a digitação requerem entrada focada. A agitação e os passos requerem movimento físico e sensores suportados. As definições de dificuldade e objetivo alteram a quantidade de trabalho esperado, mas uma missão mais difícil não é automaticamente uma melhor. A fricção excessiva pode encorajar a desativação do alarme inteiramente, enquanto uma tarefa fácil pode tornar-se automática após repetição.

Associe a tarefa ao modo de falha. Se desliga os alarmes meio adormecido, digitalizar noutro quarto cria distância útil. Se o acesso à câmara é inconveniente, uma tarefa curta de digitação ou matemática pode ser mais prática. Se houver preocupações com mobilidade, equilíbrio ou acessibilidade, evite missões baseadas em movimento e escolha uma tarefa que possa ser concluída com segurança.

## Modos único, cadeia e aleatório

O modo único pede uma missão configurada. O modo cadeia executa várias missões configuradas em ordem. O modo aleatório seleciona de um conjunto configurado, reduzindo a probabilidade de uma interação memorizada se tornar automática. Estes modos estão presentes na fonte verificada mais recente; a [disponibilidade](../availability.md) explica por que isso não prova que já estão em cada compilação pública.

Execute sempre um teste a curto prazo após alterar o modo, permissões ou objetos registados. Mantenha o objeto selecionado acessível e forneça uma rota de recuperação segura. Para problemas de entrega não relacionados com a conclusão da missão, use a [lista de verificação de fiabilidade](../help/alarm-delivery.md).

