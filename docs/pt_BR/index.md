---
title: Documentação do BarcodeWake
lang: pt_BR
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

O BarcodeWake é um despertador que torna o cancelamento um ato deliberado. Um alarme pode exigir um código de barras ou QR code salvo, uma tarefa cognitiva curta, uma sequência de sacudidas ou uma meta de passos, em vez de depender apenas de um botão fácil na tela.

## O que torna o BarcodeWake diferente

A ideia central é distância mais intenção. Se o código registrado estiverattached a um objeto longe da cama, silenciar o alarme significa levantar, alcançar esse objeto e escaneá-lo. O mesmo modelo de alarme também pode usar matemática, digitação, sacudidas ou missões de passos. O código-fonte atual suporta uma única missão, uma cadeia ordenada ou seleção aleatória de missões configuradas.

Esse atrito é útil para pessoas que cancelam um alarme comum sem se tornarem totalmente alertas. Não é análise de estágio de sono, orientação médica ou garantia de que alguém vai acordar. O suporte de hardware, permissões e controles de bateria dos fabricantes ainda afetam a entrega. A [referência de missões](features/missions.md) explica as escolhas, enquanto o [solução de problemas de entrega de alarmes](help/alarm-delivery.md) aborda as configurações do sistema que podem interferir.

## Comece com o documento correto

Use o [guia de configuração](guides/set-up-an-alarm.md) ao criar um alarme e registrar um código físico. Leia [backup e compartilhamento](guides/backup-and-sharing.md) antes de mover dados ou enviar um QR de configuração para outra pessoa. O formato de compartilhamento deliberadamente exclui códigos registrados, identificadores NFC, PINs e histórico de alarmes, então um destinatário deve concluir a configuração sensível localmente.

Para um resumo curto e auditável, veja [fatos do produto](facts.md). Para status de lançamento, use [disponibilidade](availability.md): a versão pública do Google Play capturada para esta auditoria difere da versão declarada pela árvore de código-fonte verificada. A versão mais recente do código-fonte é, portanto, documentada como capacidade do código-fonte, não afirmada como uma versão publicada na loja.

## Limites de privacidade e confiabilidade

A configuração principal e os dados de missão são armazenados no dispositivo, e nenhuma conta BarcodeWake é necessária. Os caminhos de código atuais representam valores de código registrados com hashes SHA-256. A telemetria opcional é descrita pela política de privacidade como desativada por padrão. Essas declarações não significam que todos os telefones entregarão alarmes de forma idêntica; fornecedores e permissões do sistema operacional Android ainda podem restringir o comportamento em segundo plano.

Leia [privacidade e confiabilidade](features/privacy-and-reliability.md) para a distinção entre manipulação de dados locais e entrega do sistema operacional. A [comparação com despertador padrão](comparisons/standard-alarm.md) ajuda a decidir se o cancelamento baseado em missões corresponde à forma como você acorda.

