---
icon: fontawesome/solid/layer-group
title: Webové mapové služby v prohlížeči
---

## Cíle cvičení

<div class="grid cards grid_icon_info smaller_padding" markdown> <!-- specificky format gridu (trida "grid_icon_info") na miru uvodni strance predmetu -->

-   :fontawesome-regular-handshake:{ .xl }

    __seznámení s prostředím__ webové mapové prohlížečky ZÚ (Geoprohlížeč)

-   :material-layers-triple-outline:{ .xl }

    __průzkum nabídky dat__ různých poskytovatelů

-   :material-layers-plus:{ .xl }

    __přidání mapových služeb do webové mapy__ geoportálu

-   :material-map-marker-plus-outline:{ .xl }

    __extrakce informací__ z více vrstev ke konkrétnímu místu

-   :material-lightbulb-on-10:{ .xl }

    __shrnutí a interpretace__ získaných informací

</div>

<hr class="level-1">

## Geoprohlížeč ČÚZK

__Český úřad zeměměřický a katastrální__ (ČÚZK) je státní instituce spravující katastr nemovitostí. Pod tento orgán spadá __Zeměměřický úřad__, který má na starosti mj. správu státního mapového díla (oficiální mapy ČR) a __poskytování geodetických a kartografických dat__. V rámci této služby úřad poskytuje i webovou mapovou prohlížečku – tzv. __Geoprohlížeč__ dostupný na __[této adrese](https://ags.cuzk.cz/geoprohlizec/){.underlined .external_link_icon target="_blank"}__.

![](../assets/02/img01.jpg)

<figcaption>Okno webové mapové prohlížečky "Geoprohlížeč"</figcaption>


<hr class="level-1">

## Přidávání mapových služeb

### Výběrem produktů ZÚ

Geoprohlížeč nabízí řadu __předpřipravených skupin vrstev__ pro rychlejší tvorbu mapové kompozice. Nabídka se vyvolá tlačítkem _:material-button-cursor: Produkty_{.outlined_code}. Vložená sada vrstev se objeví po kliknutí na _:material-button-cursor: Seznam vrstev_{.outlined_code}, kde lze po rozbalení __měnit viditelnost každé vrstvy zvlášť__.

!!! task-fg-color ""
    __pozor__{style="color:#c22521;" .icon-exclm .no-dec}, některé služby či skupiny vrstev mají (kvůli přehlednosti) pro každou vrstvu __přednastavené hodnoty přiblížení__, při kterých se zobrazí. Vrstva tak může být podle seznamu viditelná, ale nezobrazí se kvůli aktuálnímu přiblížení v mapě. Řešením je měnit přiblížení mapy, dokud se vrstva nezobrazí (zobrazené vrstvy jsou v seznamu zobrazeny __černým písmem__, skryté šedým písmem)

![](../assets/02/img02.png)
![](../assets/02/arrow.svg){: .off-glb .process_icon}
![](../assets/02/img03.png)
{: .process_container}

### Vložením URL adresy služby

Kromě předpřipravených datových sad lze do mapy také přidávat __libovolné služby z jiných zdrojů__ (jsou-li sdíleny v podporovaném standardu). Tomuto účelu slouží tlačítko _:material-button-cursor: Přidat vrstvy_{.outlined_code}.

![](../assets/02/img04.png)
![](../assets/02/img05.png)
{: .process_container}


<hr class="level-1">

## Extrakce informací z mapy

Atributová data mapových služeb lze číst pomocí tzv. __vyskakovacího okna__. To se objeví po __kliknutí na prvek v mapě__. V případě více viditelných překrývajících se vrstev je nutné dávat pozor, __ke které konkrétní vrstvě aktuální vyskakovací okno patří__.

![](../assets/02/img06.png)
{: .process_container}

<hr class="level-1">

!!! task-fg-color "Úloha"
    
    Následující úloha vás provede __základními úkony v rámci webové mapové aplikace Geoprohlížeč__. Pomocí __přidávání vrstev__ (mapových služeb) a __vyskakovacích oken__ budou __zjištěny informace rýzných témat__ k zadaným (skutečným) bodům v ČR.

## Zadání úlohy

Je zadán __bod o zeměpisných souřadnicích__ dle individuálního zadání:

<div class="table_no_padding table_centered" markdown>
| číslo zadání | Zeměpisná šířka (° ' '') |   |   | Zeměpisná délka (° ' '') |   |   |
| ------------ | ------------------------ | - | - | ------------------------ | - | - |
|       1      |    50   |    37   |    38,590    |    14   |    45   |    34,261    |
|       2      |    50   |    40   |    43,046    |    13   |    57   |    19,464    |
|       3      |    50   |    52   |    34,389    |    14   |    29   |    11,485    |
|       4      |    49   |     6   |     6,627    |    16   |    13   |    27,818    |
|       5      |    50   |    41   |    33,743    |    15   |    34   |    30,465    |
</div>

---

S využitím __webové mapové aplikace Geoprohlížeč__ a __mapových služeb__ či __geoportálů__ o zadaném bodu zjistěte:

<div class="annotate" markdown>

1. __příslušnost k obci__ a v jakém __katastrálním území__ bod leží

    - získejte __URL adresu mapové služby__ ArcGIS REST "Mapová služba nad daty RÚIAN" z __[Geoportálu ČÚZK](../ulohy/01.md#geoportaly "viz předchozí úloha"){.underlined_dotted}__ NEBO přidejte do mapy __předpřipravenou [sadu vrstev RÚIAN](#vyberem-produktu-zu "viz 'Přidávání mapových služeb'"){.underlined_dotted}__
    - vložte do mapy vrstvy __:material-layers: Obec__{.bg} a __:material-layers: KatastralniUzemi__{.bg} NEBO vypněte viditelnost všech ostatních vrstev __(1)__{title="trik pro hromadné zapnutí/vypnutí vrstev služby"}
    - jako odpověď uveďte hodnoty atributů __Název obce__{.outlined}, __Kód katastrálního území__{.outlined} a __Číslo katastrálního území__{.outlined}
          
---

2. __geologické podloží__ pod zadaným bodem

    - získejte __URL adresu mapové služby__ ArcGIS REST "Geologická mapa 1 : 50 000 (GEOČR50)" z webu __[České geologické služby](https://cgs.gov.cz/){.underlined_dotted .external_link_icon target="_blank"}__ (záložka "Webové služby"__(2)__{title="ukázka"}) – pozor, URL adresa mapové služby musí obsahovat klíčové slovo "rest"
    - vložte do mapy vrstvu __:material-layers: Horniny GeoČR50__{.bg}
    - jako odpověď uveďte hodnoty atributů __hornina__{.outlined} a __horninový typ__{.outlined}

---

3. adresu nejbližšího __adresního bodu__

    - získejte __URL adresu mapové služby__ ArcGIS REST "Mapová služba nad daty RÚIAN" z __[Geoportálu ČÚZK](../ulohy/01.md#geoportaly "viz předchozí úloha"){.underlined_dotted}__ NEBO přidejte do mapy __předpřipravenou [sadu vrstev RÚIAN](#vyberem-produktu-zu "viz 'Přidávání mapových služeb'"){.underlined_dotted}__
    - vložte do mapy vrstvu __:material-layers: AdresniMisto__{.bg} NEBO vypněte viditelnost všech ostatních vrstev __(3)__{title="trik pro hromadné zapnutí/vypnutí vrstev služby"}
    - jako odpověď uveďte hodnotu atributu __Adresa__{.outlined}

---

4. poštovní směrovací číslo nejbližší __pobočky České pošty__ (__pouze pobočky, ne výdejní boxy apod.__ – zde si vyzkoušíte funkci **filtrování dat**)

    - získejte __URL adresu mapové služby__ WFS z [tohoto odkazu](https://gis.cenia.cz/geoserver/pobocky_ceske_posty/wfs?SERVICE=WFS&request=GETCapabilities){.color_def .underlined_dotted .external_link_icon target="_blank"} (jedná se přímo o adresu služby, ne o webovou stránku)
    - vrstvě nastavte __filtr__ zobrazující pouze prvky, pro které atribut __`ZKR_NAZ_FUN`__ nabývá hodnot __`Podávací`, `Samostatná pošta Partner`, `Dodejna I`, `Dodejna II` a `Samostatná dodejna`__ __(4)__{title="přesný text filtru"}
    - jako odpověď uveďte pětimístné poštovní směrovací číslo nejbližší pobočky (hodnota atributu __PSC_ADRESY__{.outlined})

<!--

---

5. ~~__nadmořskou výšku lokality__~~

    - ~~výšku odečtěte ze __tří různých mapových podkladů__{.primary_color} a __výsledky porovnejte__~~
    - ~~doporučenými zdroji jsou např. 
    [__Základní topografické mapy ČR__](https://ags.cuzk.cz/geoprohlizec/ "obsahují vrstevnice s popisy výšky"){.color_def .underlined_dotted .external_link_icon target="_blank"}, webová aplikace 
    [__Analýzy výškopisu__](https://ags.cuzk.cz/av/ "režim Výpis souřadnic bodu (výškový systém Bpv (m))"){.color_def .underlined_dotted .external_link_icon target="_blank"} 
    (ČÚZK) nebo mapový portál 
    [__Mapy.cz__](https://mapy.cz/ "funkce Měření → Výškový profil"){.color_def .underlined_dotted .external_link_icon target="_blank"}~~
    - ~~jako odpověď uveďte __3 hodnoty nadmořské výšky včetně zdroje každé z nich__{.outlined}~~

-->

---

6. k jaké __změně využití území__ v zadaném bodě došlo mezi lety 1990 a 2018

    - využijte data evropského programu [__Copernicus__](https://www.copernicus.eu/cs "program EU pro družicové pozorování Země v zájmu obecného užitku všech občanů"){.color_def .underlined_dotted .external_link_icon target="_blank"} – __:material-layers: Corine Land Cover Europe__{.bg .color_def target="_blank"}
    - dostupné ze stránek &nbsp;[__Evropské agentury pro životní prostředí (EEA)__](https://land.copernicus.eu/en/products/corine-land-cover?tab=main){ .color_def .underlined_dotted .external_link_icon target="_blank"}&nbsp; či &nbsp;[__Copernicus Land Monitoring Service (CLMS)__](https://www.eea.europa.eu/en/datahub/datahubitem-view/a5144888-ee2a-4e5d-a7b0-2bbf21656348){ .color_def .underlined_dotted .external_link_icon target="_blank"}<br>
    *(Ze stránek EEA či CLMS použijte mapovou službu 'REST API', resp. 'ESRI: REST', u WMS bohužel není v tomto případě možné vyčítat hodnoty atributů vrstvy)*
    - jako odpověď uveďte __kód a slovní název__{.outlined} kategorie Land Cover pro obě období a __jejich slovní porovnání__{.outlined}

---
<!--
7. ~~zda dochází v lokalitě k překročení hodnoty 20 µg/m³ u roční průměrné koncentrace suspendovaných prachových částic PM10 a jakých hodnot v ng/m³ dosahují roční průměrné koncentrace benzoapyrenu (použijte službu III_5_7_8_CHMU_ovzdusi z ArcGIS Online, vrstva ČHMÚ ovzduší – Koncentrace látek znečišťujících ovzduší v gridu 1x1 km, rok 2019)~~

    - ~~využijte vrstvy od [__České informační agentury životního prostředí__](https://gis.cenia.cz/geoserver/chmu_ovzdusi/wfs?SERVICE=WFS&request=GETCapabilities "adresu odkazu lze přímo použít jako mapovou vrstvu"){.color_def .underlined_dotted .external_link_icon target="_blank"} (CENIA).~~

---
-->
7. jaké hodnoty dosahovala v zadané lokalitě __intenzita světelného znečištění__ v roce 2022

    
    - získejte __URL adresu mapové služby__ WMS __:material-layers: Světelné zněčištění__{.bg} z [tohoto odkazu](https://gis.cenia.cz/geoserver/svetelne_znecisteni/wms?service=WMS&request=GetCapabilities){.color_def .underlined_dotted .external_link_icon target="_blank"} (jedná se přímo o adresu služby, ne o webovou stránku). Poskytovatelem služby je [__Česká informační agentura životního prostředí__](https://cenia.gov.cz/){.underlined_dotted .external_link_icon target="_blank"} (CENIA)
    - jako odpověď uveďte __hodnotu intenzity znečištění__{.outlined} z rastru

    <!--  Puvodni vrstva ZDE: https://gis.cenia.cz/geoserver/svetelne_znecisteni/wms?service=WMS&request=GetCapabilities  -->

---

8. příslušnost zadané lokality ke __stavebnímu a matričnímu úřadu__

    - získejte __URL adresu mapové služby__ WFS __:material-layers: Působnost úřadů__{.bg} z [tohoto odkazu](https://gis.cenia.cz/geoserver/pusobnost_uradu/wfs?SERVICE=WFS&request=GETCapabilities){.color_def .underlined_dotted .external_link_icon target="_blank"} (jedná se přímo o adresu služby, ne o webovou stránku). Poskytovatelem služby je [__Česká informační agentura životního prostředí__](https://cenia.gov.cz/){.underlined_dotted .external_link_icon target="_blank"} (CENIA)
    - jako odpověď uveďte __název příslušného úřadu__{.outlined} (pro oba typy instituce)

</div>

1. <br>![](../assets/02/img07.png){ .no-filter }<br><br>__trik pro hromadné zapnutí/vypnutí vrstev služby__{style="display:block; text-align:center;"}
2. ![](../assets/02/img08.png){ .no-filter }
3. <br>![](../assets/02/img07.png){ .no-filter }<br><br>__trik pro hromadné zapnutí/vypnutí vrstev služby__{style="display:block; text-align:center;"}
4. <br>`"ZKRNAZ_FUN" IN ('Podávací','Samostatná pošta Partner','Dodejna I','Dodejna II','Samostatná dodejna')`


&nbsp;

&nbsp;
<!--
---


DALŠÍ TIPY (nalezeno na Cenii):

Světelné znečištění: https://gis.cenia.cz/geoserver/svetelne_znecisteni/wms?service=WMS&request=GetCapabilities
Úřady: https://gis.cenia.cz/geoserver/pusobnost_uradu/wms?service=WMS&request=GetCapabilities
Školy a školská zařízení: https://gis.cenia.cz/geoserver/skoly/wms?service=WMS&request=GetCapabilities
Pobočky České pošty (je tam problém, že to bere i Pošta Partner, Balíkovny a jiná místa): https://gis.cenia.cz/geoserver/pobocky_ceske_posty/wms?service=WMS&request=GetCapabilities
Ovzduší: https://gis.cenia.cz/geoserver/chmu_ovzdusi/wms?service=WMS&request=GetCapabilities

Další zajímavé vrstvy zde (ale mám problém s popupem!): https://gis.cenia.cz/geoserver/ows?service=WMS&version=1.3.0&request=GetCapabilities

ALE POZOR! VSECHNY TY VRSTVY MAJI I WFS A TA FUNGUJE!!!
STACI PREPSAT NA: https://gis.cenia.cz/geoserver/pobocky_ceske_posty/wfs?SERVICE=WFS&request=GETCapabilities
WFS jede v AGOLu i v Geoprohlizeci (paradoxne v Procku to ma trochu problemy)

zde zajimava informace o WMS: https://community.esri.com/t5/arcgis-api-for-silverlight-questions/direct-link-to-wms-sub-layer/td-p/171686

-->

<!--
&nbsp;

__Dále vytvořte a vyexportujte mapové kompozice:__



9. využití území dle __:material-layers: CORINE Land Cover 2018__{.bg} __(3)__{title="legenda Corine Land Cover"} nad __:material-layers: Základní topografickou mapou__{.bg}, __měřítko volte 1 : 10 000__ __(10)__{title="nastavení měřítka při exportu mapy"}, __formát A4 landscape__ __(1)__{title="ukázka řešení"}

    - Základní topografická mapa je k dispozici např. na [__Geoportálu ČÚZK__](https://geoportal.cuzk.cz/ "Služby → Prohlížecí → Esri ArcGIS Server (nebo WMS)"){.color_def .underlined_dotted .external_link_icon target="_blank"}, lze ji také vyhledat v prostředí [__ArcGIS Online__](https://www.arcgis.com/ "služba 'Základní topografická mapa' od uživatele 'daniel.kolias_tonaso'"){.color_def .underlined_dotted .external_link_icon target="_blank"}
    - výchozí podkladová mapa ArcGIS Online __není součástí správného výsledku__{.primary_color}. Pro správný výsledek je nutné podkladovou mapu změnit na oficiální [__Základní topografickou mapu od Zeměměřického úřadu v souřadnicovém systému S-JTSK__]("v prostředi AGOL odpovídá službě 'Základní topografické mapy ČR (S-JTSK)' od uživatele 'Zeměměřický Úřad'"){.color_def .underlined_dotted} __(7)__{title="přidejte ZTM jako podkladovou mapu"}.

---

10. nejbližšího __maloplošného chráněného území__{.underlined_dotted title="přír. památka, přír. rezervace, nár. přír. památka, nár. přír. rezervace"} přírody (nikoli okolí Vašeho bodu, ale okolí chráněného území) __s popiskem__{.primary_color} nad __:material-layers: Základní topografickou mapou__{.bg}, __měřítko kompozice a orientaci papíru A4 volte tak, aby se dané chráněné území optimálně vešlo__ __(2)__{title="ukázka řešení"}

    - využijte vrstvu z [__Geoportálu Agentury ochrany přírody a krajiny ČR__](https://gis-aopkcr.opendata.arcgis.com/){.color_def .underlined_dotted .external_link_icon target="_blank"} (AOPK), vrstvu lze vyhledat také v prostředí [__ArcGIS Online__](https://www.arcgis.com/ "služba 'Maloplošná zvláště chráněná území' od uživatele 'aopkcr'"){.color_def .underlined_dotted .external_link_icon target="_blank"}
    - výchozí podkladová mapa ArcGIS Online __není součástí správného výsledku__{.primary_color}. Pro správný výsledek je nutné podkladovou mapu změnit na oficiální [__Základní topografickou mapu od Zeměměřického úřadu v souřadnicovém systému S-JTSK__]("v prostředi AGOL odpovídá službě 'Základní topografické mapy ČR (S-JTSK)' od uživatele 'Zeměměřický Úřad'"){.color_def .underlined_dotted} __(8)__{title="přidejte ZTM jako podkladovou mapu"}.



---

-->

<!-- 
<hr class="level-1">

## Správné řešení

??? task-fg-color "Řešení"
    &nbsp;
    
-->