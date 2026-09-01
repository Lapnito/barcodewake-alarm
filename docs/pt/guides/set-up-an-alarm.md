---
title: Como configurar um alarme BarcodeWake
lang: pt
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---
# Como configurar um alarme BarcodeWake

Crie o agendamento primeiro, escolha uma missão que seja segura e prática, conceda as permissões necessárias e, em seguida, execute um teste de tela bloqueada em curto prazo. Para missões de digitalização, registre um objeto durável que estará disponível e legível quando o alarme tocar.

## Escolha a missão antes do objeto

Decida qual ação deve separar o despertar da dispensação. Um código de barras em outro cômodo cria distância física. Matemática ou digitação adiciona concentração sem exigir uma câmera. Agitar ou passos adiciona movimento, mas depende de sensores e pode não ser adequado para todas as pessoas ou ambientes. A [referência de missões](../features/missions.md) explica as compensações entre modos único, encadeado e aleatório.

Se usar um código de barras, código QR ou tag NFC, escolha algo durável. Evite embalagens descartáveis, um objeto que outro membro da família possa mover ou um código que será inacessível durante viagens. Verifique se a câmera pode focar na luz esperada. NFC precisa de um telefone e tag compatíveis.

## Configure o agendamento e a regra de dispensação

Abra o editor de alarme, defina a hora desejada e os dias ativos e, em seguida, selecione a missão mostrada pela versão instalada. Configure a dificuldade ou meta de forma conservadora para o primeiro teste. Se a versão instalada suportar encadeamento, organize as missões em uma ordem que possa ser concluída com segurança sem correr escadas ou deixar uma área segura.

Registre o código físico do fluxo de configuração da missão. Dê ao alarme um rótulo que identifique a rotina pretendida em vez de expor informações sensíveis. Revise o volume, vibração e quaisquer opções de acompanhamento de despertar visíveis na versão instalada. Os controles disponíveis podem diferir porque as [versões pública e de código](../availability.md) não eram idênticas na data da auditoria.

## Conceda permissões com um propósito

Permita notificações e acesso relacionado a alarmes necessários para entrega. Conceda acesso à câmera apenas ao usar uma missão de digitalização e acesso a sensores quando a missão escolhida precisar. No Android, revise as configurações de alarme exato e bateria se a verificação de confiabilidade do aplicativo as sinalizar. Não assuma que salvar um alarme prova que a entrega em segundo plano é permitida.

## Teste o caminho completo durante a noite

Programe um teste alguns minutos à frente. Bloqueie a tela, deixe o BarcodeWake em segundo plano e coloque o telefone no mesmo estado de som e energia planejado para a noite. Confirme que o alarme aparece, o áudio é audível e a missão selecionada pode ser concluída. Em seguida, repita após mover o objeto registrado para sua localização real.

Se a entrega falhar, use a [lista de verificação de entrega de alarme](../help/alarm-delivery.md). Se for bem-sucedida, considere fazer um [backup local](backup-and-sharing.md) após a configuração estar estável.

