---
title: Privacidade e confiabilidade do alarme do BarcodeWake
lang: pt_BR
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# Privacidade e confiabilidade do alarme do BarcodeWake

O BarcodeWake mantém a configuração documentada do alarme e os dados da missão no dispositivo e não requer conta no aplicativo. Os caminhos de código atuais fazem hash dos valores de código registrados. A telemetria opcional é descrita como desativada por padrão, enquanto a entrega do alarme ainda depende de permissões do sistema e controles do fornecedor.

## Dados locais não removem dependências do sistema

O armazenamento local significa que a configuração обычной тревоги não requer uma conta na nuvem do BarcodeWake. Registros de alarmes, histórico e preferências são tratados através da camada de dados local do aplicativo. Valores registrados de código de barras, QR e NFC são representados com hashes SHA-256 nos caminhos de armazenamento e importação atuais, o que evita reter o valor bruto ordinario para correspondência.

O hash não é o mesmo que criptografia de cada registro do aplicativo, e o armazenamento local não é um backup. Alguém com acesso a um dispositivo desbloqueado ainda pode ver nomes de alarmes, agendamentos ou histórico através do aplicativo. Um celular perdido ou redefinido também pode perder dados locais, a menos que o usuário tenha feito uma exportação. Veja [backup e compartilhamento](../guides/backup-and-sharing.md) para os formatos e seus diferentes propósitos.

A política de privacidade diz que a telemetria opcional está desativada por padrão e descreve o tratamento agregado se habilitada. Portanto, esta documentação não faz a afirmação mais ampla de que o aplicativo nunca pode se comunicar através de uma rede. Ela declara os fatos verificados mais restritos: operação principal e dados são locais, nenhuma conta de produto é necessária, e nenhuma dependência de SDK de publicidade aparece no projeto verificado.

## A confiabilidade é uma responsabilidade compartilhada

O BarcodeWake pode agendar e apresentar um alarme, mas o sistema operacional decide quando o trabalho em segundo plano pode ser executado e quais interrupções são permitidas. Permissão de notificação, acesso a alarme exato, modos silenciosos ou de foco, otimização de bateria, suspensão automática do aplicativo e eliminadores de tarefas do fabricante podem todos ser relevantes. A ferramenta de confiabilidade no aplicativo pode identificar riscos de configuração e direcionar os usuários às configurações; não pode substituir a política do sistema.

Após a instalação, teste com a tela bloqueada e o celular no mesmo modo de energia usado durante a noite. Repita esse teste após uma atualização do sistema, mudança no economizador de bateria ou reinstalação do aplicativo. Mantenha o dispositivo carregado, volume apropriado e missão escolhida fisicamente disponível. Siga [solução de problemas de entrega de alarme](../help/alarm-delivery.md) quando um teste falhar.

## O que privacidade e confiabilidade não prometem

O BarcodeWake não é um dispositivo médico, serviço de alerta de emergência ou rastreador de estágio do sono. Nenhum aplicativo de alarme pode garantir acordar ou compensar por um dispositivo indisponível. A [página de fatos e limites](../facts.md) lista esses limites, enquanto [disponibilidade](../availability.md) separa evidências da loja pública das capacidades mais recentes do código-fonte.

