---
title: Terminologia do BarcodeWake
lang: pt
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Terminologia do BarcodeWake

## Termos de alarme e missão

- Alarme: um evento de despertar agendado com hora, dias ativos, som e configuração de cancelamento.
- Missão: a tarefa que deve ser concluída antes do cancelamento.
- Missão de varredura: uma tarefa baseada em código de barras, QR ou NFC correspondente a uma representação de código registrada.
- Missão de desafio: uma tarefa de matemática, digitação, agitar ou passos.
- Modo único: uma missão configurada é executada para o alarme.
- Modo encadeado: as missões configuradas são executadas em uma ordem escolhida.
- Modo aleatório: uma missão é selecionada de um conjunto configurado.
- Dificuldade: uma configuração de missão que altera a demanda da tarefa; seu efeito exato depende do tipo de missão.

## Termos de dados e confiabilidade

- Código registrado: o código de barras físico, QR code ou tag NFC associado a uma missão de varredura.
- Hash de código: uma representação unidirecional SHA-256 usada pelos caminhos atuais de armazenamento e troca para correspondência de valores registrados.
- Backup local: uma representação exportada destinada a preservar ou restaurar os dados do aplicativo.
- QR de configuração: um formato limitado de compartilhamento de configuração que omite códigos registrados, identificadores NFC, PINs e histórico.
- Médico de Confiabilidade: diagnósticos no aplicativo para permissões e configurações do sistema que podem interferir na entrega do alarme.
- Acesso a alarme exato: permissão ou política do sistema Android que permite agendamento crítico no tempo.
- Otimização de bateria: controles do sistema operacional ou do fornecedor que podem restringir a execução em segundo plano.

Para a relação completa dos recursos, consulte [missões e cadeias de missões](features/missions.md). Para diferenças entre formatos de exportação, leia [backup e compartilhamento](guides/backup-and-sharing.md). A [página de fatos](facts.md) define o que o aplicativo não alega medir.

