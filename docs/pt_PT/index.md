---
title: Documentação do BarcodeWake
lang: pt_PT
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Documentação do BarcodeWake

BarcodeWake é um despertador que torna o seu silenciamento um ato deliberado. Um alarme pode exigir um código de barras ou código QR guardado, uma tarefa cognitiva curta, uma sequência de sacudir ou uma meta de passos, em vez de depender apenas de um botão fácil no ecrã.

## O que torna o BarcodeWake diferente

A ideia central é distância mais intenção. Se o código registado estiver ligado a um objeto fora da cama, silenciar o alarme implica levantar-se, ir até esse objeto e digitalizá-lo. O mesmo modelo de alarme também pode usar missões de matemática, digitação, sacudir ou passos. O código fonte atual suporta uma única missão, uma cadeia ordenada ou seleção aleatória de missões configuradas.

Esse atrito é útil para pessoas que silenciam um despertador normal sem ficarem totalmente alertas. Não se trata de análise de fase do sono, aconselhamento médico ou garantia de que alguém acordará. O suporte de hardware, permissões e controlos de bateria dos fornecedores ainda afetam a entrega. A [referência da missão](features/missions.md) explica as opções, enquanto a [resolução de problemas de entrega de alarmes](help/alarm-delivery.md) aborda as definições do sistema que podem interferir.

## Comece pelo documento correto

Use o [guia de configuração](guides/set-up-an-alarm.md) ao criar um alarme e registar um código físico. Leia a [cópia de segurança e partilha](guides/backup-and-sharing.md) antes de mover dados ou enviar um QR de configuração para outra pessoa. O formato de partilha exclui deliberadamente códigos registados, identificadores NFC, PINs e histórico de alarmes, pelo que o destinatário deve concluir a configuração sensível localmente.

Para um resumo curto e auditável, consulte os [factos do produto](facts.md). Para o estado de lançamento, consulte a [disponibilidade](availability.md): a versão pública do Google Play capturada para esta auditoria difere da versão declarada pela árvore de código verificada. Por isso, a versão mais recente do código fonte é documentada como capacidade do código fonte, não como uma versão publicada na loja.

## Limites de privacidade e fiabilidade

A configuração principal e os dados da missão são armazenados no dispositivo e não é necessária qualquer conta BarcodeWake. Os caminhos de código atuais representam os valores dos códigos registados com hashes SHA‑256. A telemetria opcional é descrita pela política de privacidade como desativada por predefinição. Essas afirmações não significam que todos os telemóveis entregarão alarmes de forma idêntica; fornecedores de Android e permissões do sistema operativo ainda podem restringir o comportamento em segundo plano.

Leia [privacidade e fiabilidade](features/privacy-and-reliability.md) para a distinção entre o tratamento local de dados e a entrega pelo sistema operativo. A [comparação com despertador padrão](comparisons/standard-alarm.md) ajuda a decidir se a rejeição baseada em missões corresponde à forma como acorda.

