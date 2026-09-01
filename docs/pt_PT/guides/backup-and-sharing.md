---
title: Fazer cópia de segurança e partilhar alarmes BarcodeWake em segurança
lang: pt_PT
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Fazer cópia de segurança e partilhar alarmes BarcodeWake em segurança

Utilize uma exportação JSON quando pretender preservar ou mover os dados da aplicação, um código de barras PDF impressível para recuperação, e partilha QR de configuração quando outra pessoa apenas precisa da estrutura do alarme. A partilha omite intencionalmente segredos registados e histórico.

## Escolher o formato adequado para a tarefa

A fonte atual disponibiliza diferentes percursos de troca porque cópia de segurança e partilha não são a mesma operação. Uma cópia de segurança JSON destina-se à transferência e restauração de dados estruturados. Uma cópia de segurança PDF transforma o material de recuperação num documento de código de barras impressível. Um QR de configuração é deliberadamente mais restrito: pode transmitir uma configuração de alarme limitada sem incluir valores de código de barras registados, identificadores NFC, PINs ou histórico.

Não trate um QR de configuração como uma cópia de segurança completa do dispositivo. O destinatário deve registar os seus próprios códigos físicos e rever permissões localmente. A partilha de configuração atual também limita quantos alarmes transporta, pelo que verifique o resultado importado em vez de presumir que cada agendamento foi transferido. Os [factos do produto](../facts.md) regista estes limites.

## Criar e proteger uma cópia de segurança pessoal

Utilize a ação de exportação disponível na versão instalada, escolha JSON ou a cópia de segurança impressível de acordo com o plano de recuperação, e guarde o resultado algures que controle. Uma cópia de segurança pode revelar nomes de alarmes, agendamentos e outras configurações mesmo quando valores de código brutos registados estão protegidos ou omitidos. Trate-a como dados pessoais de rotina: evite links públicos, impressoras partilhadas e canais de mensagens não fiáveis.

Após exportar, confirme que o ficheiro pode ser encontrado e que o seu carimbo temporal corresponde à cópia de segurança pretendida. Não elimine os dados originais da aplicação apenas porque um comando de exportação reportou sucesso. O teste de restauração é a única verificação fiável, mas execute-o num dispositivo seguro ou após fazer uma segunda cópia para que o próprio teste não se torne num evento de perda.

## Partilhar configuração sem partilhar segredos

Gere um QR de configuração apenas para os alarmes que o destinatário deve receber. O destinatário digitaliza-o, revê o agendamento importado e fornece o seu próprio código, etiqueta NFC ou detalhes de recuperação. Este design impede que uma configuração partilhada transfira silenciosamente a chave física que desativa o alarme de outra pessoa.

Após a importação, cada pessoa deve executar o [teste completo de configuração de alarme](set-up-an-alarm.md). Permissões, sensores e restrições do sistema operativo não são transferidos no QR. Se um alarme importado não aparecer durante o bloqueio, siga a [resolução de problemas de entrega de alarmes](../help/alarm-delivery.md).

As versões de origem e armazenamento diferiram durante esta auditoria, pelo que uma versão pública instalada pode não expor todas as opções de troca descritas aqui. [Disponibilidade](../availability.md) explica como interpretar capacidades apenas de origem.

