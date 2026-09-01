---
title: Porque é que um alarme BarcodeWake pode não tocar
lang: pt_PT
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
# Porque é que um alarme BarcodeWake pode não tocar

Um alarme guardado ainda pode ser bloqueado por definições de notificação, acesso a alarme exato, modos de foco ou silencioso, volume baixo, restrições de bateria, suspensão da aplicação ou controlos de fundo do fabricante. Verifique a entrega separadamente da análise da missão, depois execute um teste com o ecrã bloqueado.

## Primeiro, isolar a entrega do cancelamento

Crie um alarme de teste para breve com uma missão simples e deixe a aplicação em segundo plano. Bloqueie o ecrã. Se não aparecer nenhum ecrã ou som de alarme, o problema está na entrega; alterar o código de barras registado não o resolverá. Se o alarme aparecer mas a missão não puder ser concluída, a entrega funciona e o problema está na câmara, sensor, correspondência de código ou configuração da missão.

Confirme que o alarme está ativado, que o dia agendado está correto e que o fuso horário do telefone corresponde ao agendamento pretendido. Verifique o volume dos média e do alarme em vez de confiar apenas no estado do botão lateral. Reveja as regras de não incomodar ou foco, os dispositivos de áudio ligados e se o telefone foi reiniciado após a criação do alarme.

## Rever as permissões do sistema operativo

Permita notificações e qualquer acesso a alarme exato ou alarme de ecrã inteiro solicitado pela compilação instalada. Remova o BarcodeWake de listas agressivas de otimização de bateria ou de suspensão automática quando o fabricante do dispositivo oferecer esses controlos. Abra os diagnósticos de fiabilidade na aplicação e siga as definições específicas do dispositivo que identifica. A [página de privacidade e fiabilidade](../features/privacy-and-reliability.md) explica por que razão estas dependências do sistema permanecem mesmo quando os dados da aplicação são locais.

Após alterar uma definição, repita o teste com o ecrã bloqueado. Alterar vários controlos de uma só vez torna mais difícil identificar a causa. As atualizações do sistema podem redefinir ou reinterpretar permissões, por isso volte a testar após uma atualização importante ou reinstalação da aplicação.

## Diagnosticar a conclusão da missão separadamente

Para missões de código de barras e QR, limpe a lente da câmara, melhore a iluminação e confirme que o objeto registado não foi alterado. Conceda permissão à câmara. Para NFC, verifique o suporte do dispositivo e segure a etiqueta perto da posição correta da antena. Missões de agitar e passos dependem de sensores de movimento ou passos e podem comportar-se de forma diferente quando modos de economia de energia restringem a entrega do sensor.

Se uma missão foi configurada como parte de uma cadeia, cada passo necessário deve ser concluído. Reveja o [comportamento das missões](../features/missions.md) e, se necessário, crie um novo teste usando o [procedimento de configuração](../guides/set-up-an-alarm.md).

## Saber quando o telemóvel é a limitação

O BarcodeWake não pode substituir um dispositivo desligado, uma bateria esgotada, hardware de áudio avariado ou qualquer eliminado de tarefas do fabricante. Não é um serviço de notificação de emergência. Mantenha outro método de alarme para situações de alta consequência e relate falhas reproduzíveis com o modelo do dispositivo, versão do sistema, versão da aplicação e as condições exatas do teste.

