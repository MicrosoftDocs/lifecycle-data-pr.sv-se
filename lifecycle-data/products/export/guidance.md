---
title: Exportguide för livscykeldata
description: Exportguide för information om produktens livscykel
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546986"
---
# <a name="lifecycle-data-export-guidance"></a>Exportguide för livscykeldata
Det här dokumentet beskriver hur du använder produktens exportfil.

## <a name="query-information"></a>Frågeinformation
I Excel-dokumentet finns fält för att identifiera data som fylls i i produkttabellen.

### <a name="end-of-support"></a>Support upphör
Värdet Support upphör filtrerar produkterna efter datumet då support upphör eller slutdatum för lanseringen.

Möjliga värden: Alla (inget filter används), År och ett Intervall.

### <a name="family"></a>Familj
Sortimentvärdet filtrerar produkter efter överordnad nivå inom hierarkin som kallas för sortimentet.

Möjliga värden: Alla (inget filter används), sortimentnamn

### <a name="group"></a>Grupp
Gruppvärdet filtrerar produkter inom dess överordnade nivå (familj) till en viss grupp.

Möjliga värden: Alla (inget filter används), Gruppnamn

## <a name="table-columns"></a>Tabellkolumner
Produkttabellen består av kolumner som definierar produkten, utgåvor, versioner och motsvarande supportdatum.

> [!NOTE]
> Det finns en rad för varje kombination av produkt, version och utgåva.

### <a name="product"></a>Produkt
Produktnamnet.

### <a name="edition"></a>Edition
Kolumnen Version fylls i när produkten innehåller versioner. När det inte finns någon produktversion är det här fältet tomt.

### <a name="release"></a>Version
Kolumnen Utgåva fylls i när produkten innehåller flera utgåvor.
När produkten bara har en utgåva är det här fältet tomt.

### <a name="support-policy"></a>Supportpolicy
Det här fältet definierar vilken supportpolicy produkten följer.

Möjliga värden: [Fast](/lifecycle/policies/fixed), [Modern](/lifecycle/policies/modern), Komponent

### <a name="start-date"></a>Startdatum
Datum då supporten för produkten påbörjades.

### <a name="mainstream-date"></a>Mainstream-datum
När supportpolicyn är **Fast** eller **Komponent** gäller datumet som produktens mainstream-slutdatum.
  
När supportpolicyn är **modern** är fältet tomt.

### <a name="extended-end-date"></a>Utökat slutdatum
När supportpolicyn är **Fast** eller **Komponent** är det här datumet för produktens utökade slutdatum.

När supportpolicyn är **modern** är fältet tomt.

### <a name="retirement-date"></a>Avyttringsdatum
När supportpolicyn är **Fast** eller **Komponent** är det här tomt.

När supportpolicyn är **Modern** blir det här produktens avyttringsdatum.

### <a name="release-start-date"></a>Startdatum för utgåvan
Datum då supporten för versionen påbörjades. När produkten bara har en utgåva är det här fältet tomt.
 
### <a name="release-end-date"></a>Versionens slutdatum
Datum då supporten upphörde för versionen.
När produkten bara har en utgåva är det här fältet tomt.

### <a name="docs-url"></a>Url för dokument
Url för utökad dokumentation.
