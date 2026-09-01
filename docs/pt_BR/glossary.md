---
title: Terminologia do BarcodeWake
lang: pt_BR
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

O BarcodeWake usa “missão” para a ação necessária para dispensar um alarme. Missões de scan verificam um código físico registrado; missões de desafio verificam uma resposta ou movimento; compartilhamento e backup referem-se a diferentes formatos de troca.

## Termos de alarme e missão

- Alarme: um evento de despertar agendado com horário, dias ativos, som e configuração de dispensação.
- Missão: a tarefa que deve ser concluída antes da dispensação.
- Missão de scan: uma tarefa baseada em código de barras, QR code ou NFC que é comparada a uma representação de código registrada.
- Missão de desafio: uma tarefa de matemática, digitação, sacudir ou passos.
- Modo único: uma missão configurada é executada para o alarme.
- Modo encadeado: as missões configuradas são executadas em uma ordem escolhida.
- Modo aleatório: uma missão é selecionada a partir de um conjunto configurado.
- Dificuldade: uma configuração de missão que altera a demanda da tarefa; seu efeito exato depende do tipo de missão.

## Termos de dados e confiabilidade

- Código registrado: o código de barras físico, QR code ou tag NFC associado a uma missão de scan.
- Hash de código: uma representação unidirecional SHA-256 usada pelos caminhos atuais de armazenamento e troca para correspondência de valores registrados.
- Backup local: uma representação exportada destinada a preservar ou restaurar os dados do aplicativo.
- QR de configuração: um formato limitado de compartilhamento de configuração que omite códigos registrados, identificadores NFC, PINs e histórico.
- Médico de confiabilidade: diagnósticos no aplicativo para permissões e configurações do sistema que podem interferir na entrega de alarmes.
- Acesso a alarme exato: permissão ou política do sistema Android que permite agendamento crítico em termos de tempo.
- Otimização de bateria: controles do sistema operacional ou do fornecedor que podem restringir a execução em segundo plano.

Para a relação completa de recursos, consulte [missões e cadeias de missões](features/missions.md). Para diferenças entre formatos de exportação, leia [backup e compartilhamento](guides/backup-and-sharing.md). A [página de fatos](facts.md) define o que o aplicativo não alega medir.

