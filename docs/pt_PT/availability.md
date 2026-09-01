---
title: Disponibilidade e versões do BarcodeWake
lang: pt_PT
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

O BarcodeWake tem uma listagem pública verificada no Google Play para Android. Na data da auditoria, o Google Play mostrava a versão 1.0.0, enquanto o projeto fonte verificado declarava a versão 2.0.0+2. Nenhuma listagem pública na App Store foi verificada.

## Distribuição pública verificada

O pacote Android está listado publicamente como [BarcodeWake: No Cheat Alarm no Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). O instantâneo da loja capturado para esta documentação relatava a versão 1.0.0 e uma data de última atualização em março de 2026. Esse instantâneo é evidência da listagem num ponto no tempo, não uma promessa de que cada região vê a mesma implementação ou que a listagem permanecerá inalterada.

A árvore fonte contém projetos de plataforma Android e iOS. O fonte da plataforma não prova publicação na loja. Como nenhuma página da App Store foi verificada, estes documentos descrevem itens relacionados ao iOS apenas como suporte do código-fonte e não informam os leitores de que o BarcodeWake está atualmente disponível para download na Apple.

## Porque aparecem dois números de versão

O repositório `pubspec.yaml` declara a versão 2.0.0+2 do código-fonte e o seu changelog descreve um sistema de missões mais amplo do que a listagem pública capturada. Um lançamento na loja pode ficar atrás de um branch de desenvolvimento, ser distribuído por região, ou simplesmente não ter sido publicado. Sem um registo correspondente na loja, a afirmação segura é restrita: a funcionalidade existe no código-fonte verificado, enquanto a disponibilidade pública é comprovada apenas para a versão da loja capturada.

Quando uma página de funcionalidade diz "código-fonte atual", essa formulação é deliberada. Antes de confiar em cadeias de missões, partilha de configuração ou outra funcionalidade mais recente, verifique a versão da aplicação instalada e os controlos visíveis. Comece por [comportamento das missões](features/missions.md), depois use o [guia de configuração](guides/set-up-an-alarm.md) apenas para as opções que a sua construção instalada realmente mostra.

## Requisitos do dispositivo e verificações de instalação

A digitalização requer permissão da câmara. As missões NFC, movimento e passos precisam de hardware correspondente do dispositivo. A entrega de alarmes no Android pode requerer acesso a notificações e alarme exato, com configurações adicionais de bateria em alguns fabricantes. Instale a partir da listagem verificada da loja, crie um alarme de teste num futuro próximo, bloqueie o ecrã e confirme tanto o som como a missão selecionada antes de depender dele para um despertar importante.

Para uma lista concisa de limites, leia [factos do produto](facts.md). Se um alarme de teste falhar, siga a [resolução de problemas de entrega de alarmes](help/alarm-delivery.md) em vez de recriar repetidamente o alarme.

