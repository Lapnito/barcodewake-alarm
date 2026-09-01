---
title: Por que um alarme BarcodeWake pode não tocar
lang: or
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

Um alarme salvo ainda pode ser bloqueado por configurações de notificação, acesso a alarme exato, modos de foco ou silencioso, volume baixo, restrições de bateria, suspensão do aplicativo ou controles de segundo plano do fabricante. Verifique a entrega separadamente da verificação da missão, então execute um teste na tela de bloqueio.

## Primeiro isole a entrega do descarte

Crie um alarme de teste com prazo próximo com uma missão simples e deixe o aplicativo em segundo plano. Bloqueie a tela. Se nenhuma tela ou som de alarme aparecer, o problema é a entrega; alterar o código de barras registrado não resolverá. Se o alarme aparecer, mas a missão não puder ser concluída, a entrega funciona e o problema é a câmera, sensor, correspondência de código ou configuração da missão.

Confirme que o alarme está ativado, o dia agendado está correto e o fuso horário do telefone corresponde ao agendamento pretendido. Verifique o volume de mídia e de alarme em vez de confiar apenas no estado do botão lateral. Revise as regras de não perturbe ou foco, dispositivos de áudio conectados e se o telefone foi reiniciado após a criação do alarme.

## Revise as permissões do sistema operacional

Permita notificações e qualquer acesso a alarme exato ou alarme de tela cheia solicitado pela versão instalada. Remova o BarcodeWake de otimizações agressivas de bateria ou listas de suspensão automática quando o fabricante do dispositivo oferecer esses controles. Abra o diagnóstico de confiabilidade no aplicativo e siga as configurações específicas do dispositivo que ele identificar. A [página de privacidade e confiabilidade](../features/privacy-and-reliability.md) explica por que essas dependências do sistema permanecem mesmo quando os dados do aplicativo são locais.

Após alterar uma configuração, repita o teste na tela de bloqueio. Alterar vários controles de uma vez torna a causa mais difícil de identificar. Atualizações do sistema podem redefinir ou reinterpretar permissões, então teste novamente após uma atualização importante ou reinstalação do aplicativo.

## Diagnosticar a conclusão da missão separadamente

Para missões de código de barras e QR, limpe a lente da câmera, melhore a iluminação e confirme que o objeto registrado não mudou. Conceda permissão de câmera. Para NFC, verifique o suporte do dispositivo e segure a etiqueta perto da posição correta da antena. Missões de sacudir e caminhar dependem de sensores de movimento ou passos e podem se comportar de forma diferente quando modos de economia de energia restringem a entrega do sensor.

Se uma missão foi configurada como parte de uma cadeia, cada etapa necessária deve ser concluída. Revise o [comportamento das missões](../features/missions.md) e, se necessário, crie um novo teste usando o [procedimento de configuração](../guides/set-up-an-alarm.md).

## Saiba quando o telefone é o limite

O BarcodeWake não pode substituir um dispositivo desligado, bateria esgotada, hardware de áudio quebrado ou todos os eliminadores de tarefas do fabricante. Não é um serviço de notificação de emergência. Mantenha outro método de alarme para situações de alta consequência e relate falhas reproduzíveis com modelo do dispositivo, versão do sistema, versão do aplicativo e as condições exatas do teste.

