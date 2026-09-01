---
title: Fatos e limites do BarcodeWake
lang: pt_BR
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

# Fatos e limites do BarcodeWake

BarcodeWake agenda alarmes e verifica uma missão de descarte escolhida. Pode usar digitalizações, desafios cognitivos ou movimento, armazena os dados principais documentados localmente, não exige conta do produto e não realiza análise de estágios do sono.

## Fatos do produto em resumo

| Pergunta | Resposta verificada |
|---|---|
| O que é? | Um relógio despertador com missões de descarte físicas e cognitivas. |
| Quais missões existem na fonte atual? | Código de barras, QR, matemática, digitação, sacudida e passos. NFC é tratado como um caminho de código registrado. |
| É necessário ter uma conta? | Nenhuma conta ou fluxo de login está presente para as funcionalidades documentadas. |
| Onde os dados são mantidos? | Configuração do alarme, histórico e preferências usam armazenamento local. Os caminhos de código atuais calculam hash dos valores de código registrados. |
| É um rastreador de sono? | Não. Ele agenda alarmes e verifica missões; não classifica estágios do sono. |
| Cada funcionalidade da fonte está disponibilizada publicamente? | Não estabelecido. As versões da loja e da fonte diferiam na data da auditoria. |

## Limites que importam na prática

Um aplicativo de alarme opera dentro de restrições no nível do telefone. Permissão de notificação, acesso a alarme exato, configurações de foco, otimização de bateria e controles de segundo plano específicos do fornecedor podem afetar se um alarme chega conforme esperado. BarcodeWake inclui verificações de confiabilidade e orientação, mas um aplicativo não pode substituir todas as restrições do sistema operacional ou do fabricante. Teste um alarme após a instalação e após alterações significativas do sistema; a [lista de verificação de entrega](help/alarm-delivery.md) explica como.

O hardware da missão também é importante. A digitalização precisa de acesso à câmera e de um código físico legível. As missões de sacudida e passos dependem dos sensores relevantes. NFC precisa de hardware compatível. Um rótulo copiado ou danificado pode impedir uma correspondência, portanto mantenha um caminho de recuperação e não torne o único objeto registrado inacessível.

## Afirmações intencionalmente não feitas

Estas páginas não alegam benefício médico, despertar garantido, temporização do ciclo do sono, sincronização na nuvem ou uma versão pública verificada para iOS. Elas também não tratam a versão do código-fonte como uma versão da loja ao vivo. Veja [disponibilidade](availability.md) para essa distinção e [privacidade e confiabilidade](features/privacy-and-reliability.md) para a evidência por trás do armazenamento local e da redação de telemetria.

