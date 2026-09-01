---
title: Terminologia do BarcodeWake
lang: pt_PT
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

BarcodeWake utiliza “missão” para a ação necessária para dispensar um alarme. As missões de scan verificam um código físico registado; as missões de desafio verificam uma resposta ou movimento; partilha e cópia de segurança referem-se a diferentes formatos de troca.

## Termos de alarme e missão

- Alarme: um evento de despertar agendado com hora, dias ativos, som e configuração de dispensa.
- Missão: a tarefa que deve ser completada antes da dispensa.
- Missão de scan: uma tarefa baseada em código de barras, QR ou NFC que é comparada com uma representação de código registado.
- Missão de desafio: uma tarefa de matemática, digitação, shake ou contagem de passos.
- Modo único: uma missão configurada é executada para o alarme.
- Modo em cadeia: as missões configuradas são executadas numa ordem escolhida.
- Modo aleatório: uma missão é selecionada de um conjunto configurado.
- Dificuldade: uma definição de missão que altera a exigência da tarefa; o seu efeito exato depende do tipo de missão.

## Termos de dados e fiabilidade

- Código registado: o código de barras físico, código QR ou etiqueta NFC associado a uma missão de scan.
- Hash de código: uma representação unidirecional SHA‑256 utilizada pelos caminhos atuais de armazenamento e troca para correspondência com valores registados.
- Cópia de segurança local: uma representação exportada destinada a preservar ou restaurar os dados da aplicação.
- QR de configuração: um formato limitado de partilha de configuração que omite códigos registados, identificadores NFC, PINs e histórico.
- Reliability Doctor: diagnósticos na aplicação para permissões e definições do sistema que podem interferir na entrega de alarmes.
- Acesso a alarme exato: permissão ou política do sistema Android que permite o agendamento crítico no tempo.
- Otimização de bateria: controlos do sistema operativo ou do fornecedor que podem restringir a execução em segundo plano.

Para a relação completa de funcionalidades, consulte [missões e cadeias de missões](features/missions.md). Para diferenças entre formatos de exportação, leia [cópia de segurança e partilha](guides/backup-and-sharing.md). A [página de factos](facts.md) define o que a aplicação não declara medir.

