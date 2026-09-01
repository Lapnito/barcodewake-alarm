---
title: Disponibilidade e versões do BarcodeWake
lang: pt_BR
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilidade e versões do BarcodeWake

O BarcodeWake possui uma listagem pública verificada no Google Play para Android. Na data da auditoria, o Google Play mostrava a versão 1.0.0, enquanto o projeto fonte verificado declarava a versão 2.0.0+2. Nenhuma listagem pública na App Store foi verificada.

## Verified public distribution

O pacote Android está listado publicamente como [BarcodeWake: No Cheat Alarm no Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). O snapshot da loja capturado para esta documentação relatava a versão 1.0.0 e uma data de última atualização em março de 2026. Esse snapshot é evidência da listagem em um ponto no tempo, não uma promessa de que todas as regiões veem o mesmo lançamento ou que a listagem permanecerá inalterada.

A árvore fonte contém projetos de plataforma Android e iOS. O fonte da plataforma não prova publicação na loja. Como nenhuma página da App Store foi verificada, estes docs descrevem itens relacionados ao iOS apenas como suporte de código fonte e não informam aos leitores que o BarcodeWake está atualmente disponível para download na Apple.

## Why two version numbers appear

O repositório `pubspec.yaml` declara a versão fonte 2.0.0+2 e seu changelog descreve um sistema de missões mais amplo do que a listagem pública capturada. Um lançamento na loja pode ficar atrás de uma branch de desenvolvimento, ser distribuído por região, ou simplesmente não ter sido publicado. Sem um registro correspondente na loja, a afirmação segura é restrita: a funcionalidade existe no fonte verificado, enquanto a disponibilidade pública é comprovada apenas para a versão da loja capturada.

Quando uma página de funcionalidade diz "código fonte atual", essa redação é deliberada. Antes de confiar em cadeias de missões, compartilhamento de configuração ou outra funcionalidade mais recente, verifique a versão do aplicativo instalado e os controles visíveis. Comece com o [comportamento das missões](features/missions.md), depois use o [guia de configuração](guides/set-up-an-alarm.md) apenas para as opções que sua build instalada realmente mostra.

## Device requirements and installation checks

A leitura requer permissão da câmera. Missões de NFC, movimento e passos precisam de hardware correspondente no dispositivo. A entrega de alarmes no Android pode requerer acesso a notificações e alarme exato, com configurações adicionais de bateria em alguns fabricantes. Instale a partir da listagem verificada da loja, crie um alarme de teste para breve, bloqueie a tela e confirme tanto o som quanto a missão selecionada antes de depender dele para um despertar importante.

Para uma lista concisa de limitações, leia os [fatos do produto](facts.md). Se um alarme de teste falhar, siga o [diagnóstico de problemas de entrega de alarmes](help/alarm-delivery.md) em vez de recriar o alarme repetidamente.

