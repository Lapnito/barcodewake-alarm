---
title: Factos e limites do BarcodeWake
lang: pt_PT
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Factos e limites do BarcodeWake

O BarcodeWake agenda alarmes e verifica uma missão de desmistificação escolhida. Pode usar digitalizações, desafios cognitivos ou movimento, armazena os dados principais documentados localmente, não requer uma conta de produto e não executa análise de etapas de sono.

## Factos do produto num relance

| Pergunta | Resposta verificada |
|---|---|
| O que é? | Um despertador com missões de desmistificação física e cognitiva. |
| Que missões existem na fonte atual? | Código de barras, QR, matemática, digitação, sacudir e passos. NFC é tratado como um caminho de código registado. |
| É necessária uma conta? | Nenhum fluxo de conta ou início de sessão está presente para as funcionalidades documentadas. |
| Onde são guardados os dados? | Configuração de alarme, histórico e preferências usam armazenamento local. Os caminhos de código atuais fazem hash dos valores de código registados. |
| É um rastreador de sono? | Não. Programa alarmes e verifica missões; não classifica etapas de sono. |
| Cada funcionalidade da fonte está publicamente disponível? | Não estabelecido. As versões da loja e da fonte diferiam na data de auditoria. |

## Limites que importam na prática

Uma aplicação de alarme opera dentro de restrições a nível do telemóvel. Permissão de notificação, acesso a alarme exato, definições de foco, otimização de bateria e controlos de fundo específicos do fornecedor podem afetar se um alarme chega conforme esperado. O BarcodeWake inclui verificações de fiabilidade e orientação, mas uma aplicação não pode ignorar cada restrição do sistema operativo ou fabricante. Teste um alarme após a instalação e após alterações importantes do sistema; a [lista de verificação de entrega](help/alarm-delivery.md) explica como.

O hardware das missões também importa. A digitalização requer acesso à câmara e um código físico legível. As missões de sacudir e passos dependem dos sensores relevantes. NFC requer hardware compatível. Uma etiqueta copiada ou danificada pode impedir uma correspondência, por isso mantenha um caminho de recuperação e não torne o único objeto registado inacessível.

## Afirmações intencionalmente não feitas

Estas páginas não afirmam benefício médico, despertar garantido, temporização de ciclo de sono, sincronização em nuvem ou uma versão iOS pública verificada. Também não tratam a versão da fonte como uma versão da loja ao vivo. Veja [disponibilidade](availability.md) para essa distinção e [privacidade e fiabilidade](features/privacy-and-reliability.md) para a evidência por trás do armazenamento local e formulação de telemetria.

