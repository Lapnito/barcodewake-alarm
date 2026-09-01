---
title: Fatti u limitazzjonijiet ta' BarcodeWake
lang: ml
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
# Fatti u limitazzjonijiet ta' BarcodeWake

BarcodeWake jippjana allarmi u jverifika mission magħżula ta' tneħħija. Jista' juża skannjar, sfidi konjittivi jew moviment, jaħżen id-dejta bażika ddokumentata lokali, ma jeħtiġx kont tal-prodott, u ma twettaqx analiżi tal-istadji tas-swief.

## Fatti tal-prodott f'ħarsa waħda

| Mistoqsija | Risposta verifikata |
|---|---|
| X'inhu? | Allarm li jinvolvi missioni ta' tneħħija fiżiċi u konjittivi. |
| Liema missioni jeżistu fis-sors attwali? | Barcode, QR, matematiċi, tipjar, ħarba u passi. NFC jiġi mmaniġġjat bħala triq ta' kodiċi rreġistrat. |
| Huwa kont meħtieġ? | Le, ma hemm l-ebda kont jew fluss ta' login għall-karatteristiċi ddokumentati. |
| Fejn jinħażen id-data? | Konfigurazzjoni tal-allarm, storja u preferenzi jużaw ħażna lokali. Triqiet kurrenti tal-kodiċi jagħmlu hash tal-valuri tal-kodiċi rreġistrati. |
| Huwa tracker tas-sewda? | Le. Jippjana allarmi u jverifika missioni; ma jklassifikax stadji tas-swief. |
| Kull karatteristika tas-sors ippubblikata pubblikament? | Mhux stabbilit. Verżjonijiet tal-ħanut u tas-sors kienu differenti fid-data tal-awdit. |

## Limitazzjonijiet li huma importanti fil-prattika

App ta' allarm taħdem fi ħdan limitazzjonijiet tal- telefon. Permess ta' notifika, aċċess għall-alarm preċiż, settings tal-focus, ottimizzazzjoni tal-batterija u kontrolli tal-background speċifiċi tal-manifattur jistgħu jaffettwaw jekk allarm jasal kif mistenni. BarcodeWake jinkludi kontrolli ta' affidabbiltà u gwida, iżda app ma tistax tbaxxa kull restrizzjoni tas-sistema operattiva jew tal-manifattur. Testja allarm wara l-installazzjoni u wara bidliet kbar tas-sistema; il-[lista ta' verifika tal-konsinna](help/alarm-delivery.md) tispjega kif.

Il-hardware tal-mission ukoll huwa importanti. Skannjar jeħtieġ aċċess għall-kamera u kodiċi fiżiku li jista' jinqara. Missioni ta' ħarba u passi jiddependu mis-sensors relevanti. NFC jeħtieġ hardware kompatibbli. Tikketta kopjata jew bil-ħsara tista' timpedixxi qbil, għalhekk żomm triq ta' ripristino u tiżgura li l-oġġett rreġistrat biss ma jsirx inaċċessibbli.

## Talbiet intenzjonalment mhux magħmula

Dawn il-paġni ma jikkwotawx benefiċċju mediċu, qawwa garantita ta' tqajjim, tmingħa taċ-ċiklu tas-swief, sinjalazzjoni tas-sħab jew-release pubbliku verifikat ta' iOS. Huma ukoll ma jqisux il-verżjoni tas-sors bħala verżjoni tal-ħanut ħaj. Ara [disponibbiltà](availability.md) għal dik id-distinzjoni u [privatezza u affidabbiltà](features/privacy-and-reliability.md) għall-evidenza warajh tal-ħażna lokali u l-kliem tat-telemetrija.

