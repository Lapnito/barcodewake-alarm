---
title: Por que um alarme BarcodeWake pode não tocar
lang: pt
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Por que um alarme BarcodeWake pode não tocar

Um alarme salvo ainda pode ser bloqueado por configurações de notificação, acesso a alarme exato, modos de foco ou silencioso, volume baixo, restrições de bateria, suspensão do aplicativo ou controles de fundo do fornecedor. Verifique a entrega separadamente da varredura da missão e, em seguida, execute um teste com a tela bloqueada.

## Primeiro isole a entrega da rejeição

Crie um alarme de teste de curto prazo com uma missão simples e deixe o aplicativo em segundo plano. Bloqueie a tela. Se nenhuma tela ou som de alarme aparecer, o problema é a entrega; alterar o código de barras registrado não o resolverá. Se o alarme aparecer, mas a missão não puder ser concluída, a entrega funciona e o problema está na câmera, no sensor, na correspondência do código ou na configuração da missão.

Confirme que o alarme está ativado, o dia agendado está correto e o fuso horário do telefone corresponde ao agendamento pretendido. Verifique o volume de mídia e do alarme em vez de confiar apenas no estado do botão lateral. Revise as regras de não perturbe ou foco, dispositivos de áudio conectados e se o telefone foi reiniciado após a criação do alarme.

## Revisar os controles de permissão do sistema operacional

Permita notificações e qualquer acesso a alarme exato ou de tela cheia solicitado pela versão instalada. Remova o BarcodeWake de otimização agressiva de bateria ou listas de suspensão automática quando o fornecedor do dispositivo oferecer esses controles. Abra os diagnósticos de confiabilidade no aplicativo e siga as configurações específicas do dispositivo que ele identificar. A [página de privacidade e confiabilidade](../features/privacy-and-reliability.md) explica por que essas dependências do sistema permanecem mesmo quando os dados do aplicativo são locais.

Após alterar uma configuração, repita o teste com a tela bloqueada. Alterar vários controles de uma só vez dificulta a identificação da causa. Atualizações do sistema podem redefinir ou reinterpretar permissões, portanto, teste novamente após uma atualização importante ou reinstalação do aplicativo.

## Diagnosticar a conclusão da missão separadamente

Para missões de código de barras e QR, limpe a lente da câmera, melhore a iluminação e confirme que o objeto registrado não mudou. Conceda permissão de câmera. Para NFC, verifique o suporte do dispositivo e segure a etiqueta próxima à posição correta da antena. Missões de sacudir e passo dependem de sensores de movimento ou de passos e podem se comportar de maneira diferente quando modos de economia de energia restringem a entrega do sensor.

Se uma missão foi configurada como parte de uma cadeia, cada etapa necessária deve ser concluída. Revise o [comportamento da missão](../features/missions.md) e, se necessário, crie um novo teste usando o [procedimento de configuração](../guides/set-up-an-alarm.md).

## Saber quando o celular é o limite

BarcodeWake não pode substituir um dispositivo desligado, uma bateria esgotada, hardware de áudio quebrado ou qualquer eliminador de tarefas do fabricante. Não é um serviço de notificação de emergência. Mantenha outro método de alarme para situações de alta consequência e relate falhas reprodutíveis com o modelo do dispositivo, versão do sistema, versão do aplicativo e as condições exatas do teste.

