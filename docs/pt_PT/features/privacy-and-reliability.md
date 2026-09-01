---
title: Privacidade e fiabilidade de alarmes do BarcodeWake
lang: pt_PT
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
# Privacidade e fiabilidade de alarmes do BarcodeWake

O BarcodeWake mantém a configuração de alarmes documentada e os dados da missão no dispositivo e não requer uma conta de aplicação. Os caminhos de código atuais realizam hash dos valores de código registados. A telemetria opcional é descrita como desativada por defeito, enquanto a entrega de alarmes ainda depende de permissões do sistema e de controlos do fabricante.

## Os dados locais não eliminam dependências do sistema

O armazenamento local significa que a configuração normal de alarmes não requer uma conta cloud do BarcodeWake. Os registos de alarmes, histórico e preferências são geridos através da camada de dados local da aplicação. Os valores de código de barras, QR e NFC registados são representados com hashes SHA-256 nos caminhos de armazenamento e importação atuais, o que evita manter o valor bruto original para correspondência.

O hashing não é o mesmo que a encriptação de todos os registos da aplicação, e o armazenamento local não é uma cópia de segurança. Alguém com acesso a um dispositivo desbloqueado ainda pode ver nomes de alarmes, horários ou histórico através da aplicação. Um telemóvel perdido ou reiniciado também pode perder dados locais, a menos que o utilizador tenha feito uma exportação. Consulte [cópia de segurança e partilha](../guides/backup-and-sharing.md) para os formatos e os seus diferentes objetivos.

A política de privacidade indica que a telemetria opcional está desativada por defeito e descreve o tratamento agregado se estiver ativada. Por conseguinte, esta documentação não faz a afirmação mais ampla de que a aplicação nunca pode comunicar através de uma rede. Afirma os factos verificados mais restritos: a operação principal e os dados são locais, não é necessária uma conta de produto e não aparece nenhuma dependência de SDK publicitário no projeto analisado.

## A fiabilidade é uma responsabilidade partilhada

O BarcodeWake pode agendar e apresentar um alarme, mas o sistema operativo decide quando o trabalho em segundo plano pode ser executado e quais as interrupções são permitidas. A permissão de notificação, o acesso a alarme exato, os modos silencioso ou de foco, a otimização da bateria, a suspensão automática da aplicação e os eliminadores de tarefas do fabricante podem todos ter relevância. A ferramenta de fiabilidade integrada na aplicação pode identificar riscos de configuração e direcionar os utilizadores para as definições; não pode substituir a política do sistema.

Após a instalação, teste com o ecrã bloqueado e o telemóvel no mesmo modo de energia utilizado durante a noite. Repita esse teste após uma atualização do sistema, alteração do modo de economia de bateria ou reinstalação da aplicação. Mantenha o dispositivo carregado, o volume adequado e a missão escolhida fisicamente disponível. Siga a [resolução de problemas de entrega de alarmes](../help/alarm-delivery.md) quando um teste falha.

## O que a privacidade e a fiabilidade não prometem

O BarcodeWake não é um dispositivo médico, serviço de alerta de emergência ou monitor de fase do sono. Nenhuma aplicação de alarme pode garantir que acorda ou compensar um dispositivo indisponível. A [página de factos e limites](../facts.md) lista estes limites, enquanto a [disponibilidade](../availability.md) separa a evidência da loja pública das capacidades mais recentes do código fonte.

