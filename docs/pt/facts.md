---
title: Fatos e limites do BarcodeWake
lang: pt
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

BarcodeWake agenda alarmes e verifica uma missão de dispensação escolhida. Ele pode usar escaneamentos, desafios cognitivos ou movimento, armazena os dados principais documentados localmente, não requer conta do produto e não executa análise de estágio do sono.

## Fatos do produto em resumo

| Pergunta | Resposta verificada |
|---|---|
| O que é? | Um despertador com missões de dispensação física e cognitiva. |
| Quais missões existem na fonte atual? | Código de barras, QR, matemática, digitação, sacudir e passos. NFC é tratado como um caminho de código registrado. |
| É necessária uma conta? | Nenhuma conta ou fluxo de login está presente para os recursos documentados. |
| Onde os dados são mantidos? | Configuração de alarme, histórico e preferências usam armazenamento local. Os caminhos de código atuais fazem hash dos valores de código registrados. |
| É um rastreador de sono? | Não. Ele agenda alarmes e verifica missões; não classifica estágios do sono. |
| Todos os recursos da fonte estão disponíveis publicamente? | Não estabelecido. As versões da loja e da fonte diferiam na data da auditoria. |

## Limites que importam na prática

Um aplicativo de alarme opera dentro de restrições no nível do telefone. Permissão de notificação, acesso a alarme exato, configurações de foco, otimização de bateria e controles de segundo plano específicos do fornecedor podem afetar se um alarme chega conforme esperado. BarcodeWake inclui verificações de confiabilidade e orientação, mas um aplicativo não pode substituir cada restrição do sistema operacional ou fabricante. Teste um alarme após a instalação e após grandes mudanças no sistema; a [lista de verificação de entrega](help/alarm-delivery.md) explica como.

O hardware da missão também importa. O escaneamento precisa de acesso à câmera e um código físico legível. As missões de sacudir e passos dependem dos sensores relevantes. NFC precisa de hardware compatível. Um rótulo copiado ou danificado pode impedir uma correspondência, então mantenha um caminho de recuperação e não torne o único objeto registrado inacessível.

## Afirmações intencionalmente não feitas

Essas páginas não afirmam benefício médico, despertar garantido, temporização de ciclo de sono, sincronização na nuvem ou uma versão pública verificada do iOS. Elas também não tratam a versão da fonte como uma versão da loja ao vivo. Veja [disponibilidade](availability.md) para essa distinção e [privacidade e confiabilidade](features/privacy-and-reliability.md) para a evidência por trás do armazenamento local e da redação de telemetria.

