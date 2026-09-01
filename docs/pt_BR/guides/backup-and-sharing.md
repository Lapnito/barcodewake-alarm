---
title: Fazer backup e compartilhar alarmes do BarcodeWake com segurança
lang: pt_BR
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
# Fazer backup e compartilhar alarmes do BarcodeWake com segurança

Use uma exportação JSON ao preservar ou mover seus próprios dados do aplicativo, um código de barras de backup em PDF para recuperação, e compartilhamento de QR de configuração quando outra pessoa precisa apenas da estrutura do alarme. O compartilhamento omite intencionalmente segredos registrados e histórico.

## Escolha o formato adequado para cada situação

A fonte atual oferece diferentes caminhos de troca porque backup e compartilhamento não são a mesma operação. Um backup JSON é destinado à transferência e restauração estruturada de dados. Um backup em PDF transforma o material de recuperação em um documento de código de barras para impressão. Um QR de configuração é deliberadamente mais restrito: pode passar uma configuração limitada de alarme sem carregar valores de código de barras registrados, identificadores NFC, PINs ou histórico.

Não trate um QR de configuração como um backup completo do dispositivo. O destinatário deve registrar seus próprios códigos físicos e revisar as permissões localmente. O compartilhamento de configuração atual também limita quantos alarmes ele carrega, então verifique o resultado importado em vez de presumir que cada agendamento foi transferido. Os [fatos do produto](../facts.md) registram esses limites.

## Criar e proteger um backup pessoal

Use a ação de exportação disponível na versão instalada, escolha JSON ou o backup para impressão de acordo com o plano de recuperação, e salve o resultado em algum lugar que você controla. Um backup pode revelar nomes de alarmes, agendamentos e outras configurações, mesmo quando valores brutos de códigos registrados são protegidos ou omitidos. Trate-o como dados pessoais de rotina: evite links públicos, impressoras compartilhadas e canais de mensagens não confiáveis.

Após exportar, confirme que o arquivo pode ser encontrado e que seu carimbo de data/hora corresponde ao backup pretendido. Não exclua os dados originais do aplicativo apenas porque um comando de exportação relatado sucesso. O teste de restauração é a única verificação confiável, mas execute-o em um dispositivo seguro ou após fazer uma segunda cópia para que o próprio teste não se torne um evento de perda.

## Compartilhar configuração sem compartilhar segredos

Gere um QR de configuração apenas para os alarmes que o destinatário deve receber. O destinatário digitaliza, revisa o agendamento importado e fornece seu próprio código, tag NFC ou detalhes de recuperação. Este design impede que uma configuração compartilhada transfira silenciosamente a chave física que desativa o alarme de outra pessoa.

Após a importação, cada pessoa deve executar o [teste completo de configuração de alarme](set-up-an-alarm.md). Permissões, sensores e restrições do sistema operacional não são transferidos no QR. Se um alarme importado não aparecer enquanto estiver bloqueado, siga a [solução de problemas de entrega de alarme](../help/alarm-delivery.md).

As versões da fonte e da loja diferiram durante esta auditoria, então uma versão pública instalada pode não expor todas as opções de troca descritas aqui. [Disponibilidade](../availability.md) explica como interpretar recursos disponíveis apenas na fonte.

