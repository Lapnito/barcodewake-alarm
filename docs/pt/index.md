---
title: BarcodeWake documentação
lang: pt
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---

# BarcodeWake documentação

BarcodeWake é um despertador que torna a ação de ignorar um ato deliberado. Um alarme pode exigir um código de barras ou QR code salvo, uma tarefa cognitiva breve, uma sequência de sacudidas ou uma meta de passos, em vez de depender apenas de um simples botão na tela.

## O que torna o BarcodeWake diferente

A ideia central é distância mais intenção. Se o código registrado estiver preso a um objeto longe da cama, silenciar o alarme significa levantar, alcançar esse objeto e escaneá-lo. O mesmo modelo de alarme também pode usar tarefas de matemática, digitação, sacudidas ou passos. O código-fonte atual suporta uma única missão, uma corrente ordenada ou seleção aleatória de missões configuradas.

Esse atrito é útil para pessoas que ignoram um alarme comum sem se tornarem totalmente alertas. Não se trata de análise de estágio do sono, orientação médica ou garantia de que alguém vai acordar. O suporte de hardware, permissões e controles de bateria do fornecedor ainda afetam a entrega. A [referência da missão](features/missions.md) explica as opções, enquanto a [resolução de problemas de entrega de alarme](help/alarm-delivery.md) aborda configurações do sistema que podem interferir.

## Comece com o documento certo

Use o [guia de configuração](guides/set-up-an-alarm.md) ao criar um alarme e registrar um código físico. Leia [backup e compartilhamento](guides/backup-and-sharing.md) antes de mover dados ou enviar um QR de configuração para outra pessoa. O formato de compartilhamento deliberadamente exclui códigos registrados, identificadores NFC, PINs e histórico de alarmes, portanto, o destinatário deve concluir a configuração sensível localmente.

Para um resumo curto e auditável, consulte [informações do produto](facts.md). Para o status de lançamento, use [disponibilidade](availability.md): a versão pública do Google Play capturada para esta auditoria difere da versão declarada pela árvore do código-fonte verificada. A versão mais recente do código-fonte é, portanto, documentada como capacidade da fonte, não afirmada como uma release publicada na loja.

## Limites de privacidade e confiabilidade

A configuração principal e os dados da missão são armazenados no dispositivo e nenhuma conta BarcodeWake é necessária. Os caminhos de código atuais representam valores de código registrados com hashes SHA-256. A telemetria opcional é descrita pela política de privacidade como desativada por padrão. Essas declarações não significam que todos os telefones entregarão alarmes de forma idêntica; fornecedores de Android e permissões do sistema operacional ainda podem restringir o comportamento em segundo plano.

Leia [privacidade e confiabilidade](features/privacy-and-reliability.md) para a distinção entre manipulação local de dados e entrega do sistema operacional. A [comparação com alarme padrão](comparisons/standard-alarm.md) ajuda a decidir se a dispensação baseada em missões corresponde à forma como você acorda.

