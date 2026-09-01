---
title: Como configurar um alarme BarcodeWake
lang: pt_PT
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

Crie primeiro o agendamento, escolha uma missão segura e prática, conceda as permissões necessárias e, em seguida, realize um teste bloqueado de curto prazo. Para missões de digitalização, registe um objeto durável que esteja disponível e legível quando o alarme tocar.

## Escolha a missão antes do objeto

Decida qual ação deve separar o acordar da rejeição. Um código de barras noutra sala cria distância física. Matemática ou digitação adiciona concentração sem necessitar de câmara. Agitar ou passos adiciona movimento, mas depende de sensores e pode não ser adequado para todas as pessoas ou ambientes. A [referência da missão](../features/missions.md) explica as desvantagens entre os modos único, em cadeia e aleatório.

Se utilizar um código de barras, código QR ou etiqueta NFC, escolha algo durável. Evite embalagens descartáveis, um objeto que outro membro da casa possa mover ou um código que fique inacessível durante viagens. Verifique se a câmara consegue focar na luz esperada. O NFC necessita de um telemóvel e etiqueta compatíveis.

## Configure o agendamento e a regra de rejeição

Abra o editor de alarmes, defina a hora desejada e os dias ativos e, em seguida, selecione a missão mostrada pela versão instalada. Configure a dificuldade ou o alvo de forma conservadora para o primeiro teste. Se a versão instalada suportar cadeias, organize as missões numa ordem que possa ser concluída com segurança, sem correr pelas escadas ou sair de uma área segura.

Registe o código físico a partir do fluxo de configuração da missão. Dê ao alarme uma etiqueta que identifique a rotina pretendida, em vez de expor informações sensíveis. Reveja o volume, a vibração e quaisquer opções de seguimento de despertar visíveis na versão instalada. Os controlos disponíveis podem diferir porque as [versões pública e de código](../availability.md) não eram idênticas na data da auditoria.

## Conceda permissões com um propósito

Permita notificações e acesso relacionado com alarmes necessário para a entrega. Conceda acesso à câmara apenas quando utilizar uma missão de digitalização e acesso a sensores quando a missão escolhida o exigir. No Android, rever as definições de alarme exato e bateria se a verificação de fiabilidade da aplicação os marcar. Não assuma que guardar um alarme prova que a entrega em segundo plano é permitida.

## Teste o caminho completo durante a noite

Programe um teste alguns minutos à frente. Bloqueie o ecrã, deixe o BarcodeWake em segundo plano e coloque o telemóvel no mesmo estado de som e energia planeado para a noite. Confirme que o alarme aparece, o áudio é audível e a missão exatamente selecionada pode ser concluída. Depois repita após mover o objeto registado para a sua localização real.

Se a entrega falhar, utilize a [lista de verificação de entrega de alarme](../help/alarm-delivery.md). Se for bem‑sucedida, considere fazer uma [cópia de segurança local](backup-and-sharing.md) após a configuração estar estável.

