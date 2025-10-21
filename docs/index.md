
# Adaptace krajiny na klimatickou změnu {: .page_title}




Popis úloh a nějaký celkový úvod na 2-3 odstavce? **Doplnit!**
<!--
Předmět vás seznámí se základy tzv. __geografických informačních systémů__ (GIS). GIS je soubor nástrojů sloužících ke __sběru__, __správě__, __analýze__ a __vizualizaci__ geografických dat. Umožňuje efektivně pracovat s prostorovými informacemi, což zahrnuje __mapy__, __satelitní snímky__, __adresy__, __topografické údaje__ a mnoho dalšího. Dokáže provádět složité analýzy, identifikovat vzory, a tím __lépe porozumět geografickým jevům a vztahům__.

GIS má široké uplatnění, od __:fontawesome-solid-tree-city: městského plánování__{.underlined}, přes __:fontawesome-solid-hands-holding-circle: správu přírodních zdrojů__{.underlined} až po __:fontawesome-solid-triangle-exclamation: krizový management__{.underlined}. Je nepostradatelným nástrojem pro __efektivní rozhodování a řízení__ v různých odvětvích a pomáhá lépe __pochopit složité geografické souvislosti__.
-->

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
Section 1.10.32 of "de Finibus Bonorum et Malorum", written by Cicero in 45 BC

"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"
1914 translation by H. Rackham

<figure markdown>
![](../assets/index/uvodni-foto-krajina.jpg)
</figure>


<h2 style="text-align:center;">Naučíte se</h2>
<!-- styl je zde pridany HTML tagem (ne pomoci '##'), aby se text neobjevil v tabulce obsahu vlevo na strance -->

<div class="grid cards grid_icon_info smaller_padding" markdown> <!-- specificky format gridu (trida "grid_icon_info") na miru uvodni strance predmetu -->

-   :material-database-import-outline:{ .xl }

    pracovat s __geoprostorovými daty__ vašeho města

-   :octicons-gear-16:{ .xl }

    __základní zpracování__ a __analýzu__ geoprostorových dat

-   :material-brush-variant:{ .xl }

    základy __3D tisku__ krajiny

-   :octicons-share-16:{ .xl }

    vytvářet vlastní __mapy__ 

</div>



<hr class="level-1">

<h2 style="text-align:center;">QGIS – práce s otevřeným GIS softwarem</h2>



<div class="grid cards grid_icon_info smaller_padding" markdown>

- :fontawesome-solid-map-location-dot:{ .xl }  
  __seznámení s prostředím__ open-source GIS programu QGIS  

- :material-database-outline:{ .xl }  
  __načítání a práce s daty__ z různých zdrojů (vektorová i rastrová)  

- :material-map-check-outline:{ .xl }  
  __vizualizace a analýza prostorových dat__  

- :material-file-export-outline:{ .xl }  
  __vytvoření mapové kompozice__ a její export do PDF  

</div>


<h3 style="text-align:center;">Co je QGIS</h3>


[__QGIS (Quantum GIS)__](https://qgis.org/){.color_def .underlined_dotted .external_link_icon target="_blank"} je __otevřený a bezplatný geografický informační systém (GIS)__ určený pro práci s prostorovými daty.  
Umožňuje __vytvářet, upravovat, analyzovat a vizualizovat geografická data__ podobně jako profesionální komerční systémy (např. ArcGIS).  
QGIS využívají nejen studenti a vědci, ale také odborníci z praxe — například v oblasti __geodézie, stavebnictví, územního plánování__ nebo __ochrany životního prostředí__.  

Program běží na všech běžných operačních systémech (Windows, macOS, Linux) a díky své otevřenosti podporuje širokou škálu datových formátů a služeb (např. __Shapefile, GeoPackage, GeoJSON, WMS, WFS__ aj.).  


<figure markdown>
![](../assets/index/qgis-ukazka.jpg){ width="800" }
    <figcaption>Uživatelské rozhraní QGIS – příklad mapového projektu s vektorovými vrstvami</figcaption>
</figure>


<h3 style="text-align:center;">Využití v geomatice a stavebnictví</h3>

QGIS má významné uplatnění i ve studijních programech Fakulty stavební ČVUT, zejména v oborech [__Geodézie a kartografie__](https://geomatics.fsv.cvut.cz/) a [__Stavby, krajina a životní prostředí__](https://krajina.fsv.cvut.cz/).  
Studenti zde mohou pomocí QGIS:

- analyzovat prostorové vztahy (např. __vzdálenosti, překryvy, plochy__),  
- vytvářet tematické mapy (např. __geologické podloží, druhy využití území__),  
- kombinovat data z různých zdrojů (např. __katastrální mapy, ortofoto, data o dopravní infrastruktuře__),  
- modelovat dopady stavebních záměrů na __krajinu či životní prostředí__.  

QGIS tak pomáhá propojit teoretické znalosti s praktickým využitím dat při __navrhování staveb__, __územní analýze__ nebo __hodnocení environmentálních dopadů__.  


<h3 style="text-align:center;">Proč QGIS?</h3>


<div class="grid cards" markdown>

- :material-lock-open-outline:{ .lg .middle } __Otevřený software__  
  Bez licenčních poplatků, volně dostupný a podporovaný rozsáhlou komunitou uživatelů a vývojářů.

- :simple-gitextensions:{ .lg .middle } __Rozšiřitelnost pomocí pluginů__  
  Pomocí doplňků lze přidávat nové funkce – např. propojení s CAD formáty, analýzy viditelnosti nebo export dat do 3D.

- :material-earth:{ .lg .middle } __Podpora webových mapových služeb__  
  Snadné připojení k datům z geoportálů, např. [ČÚZK](https://geoportal.cuzk.cz/){.external_link_icon target="_blank"} nebo [AOPK ČR](https://gis-aopkcr.opendata.arcgis.com/){.external_link_icon target="_blank"}.

- :material-map-search-outline:{ .lg .middle } __Vizuální analýzy__  
  Přehledná tvorba map, symbolika podle atributů, průhlednost vrstev či tisk mapových výstupů do PDF.

</div>


<h3 style="text-align:center;">Tipy pro začátek</h3>

- nainstalujte aktuální verzi z [__oficiálních stránek QGIS__](https://qgis.org/){.color_def .underlined_dotted .external_link_icon target="_blank"}  
- doporučené formáty pro práci: __GeoPackage__ (moderní a univerzální), případně __Shapefile__  
- zobrazení dat z webových zdrojů: nabídka __„Vrstva → Přidat vrstvu → Přidat WMS/WMTS nebo WFS“__  
- využijte __panel „Tiskové kompozice“__ k vytvoření mapového výstupu s měřítkem, legendou a titulkem  


<h3 style="text-align:center;">Shrnutí</h3>

QGIS představuje __dostupný a výkonný nástroj pro práci s geografickými daty__, vhodný jak pro výuku, tak pro praktické využití v technických a environmentálních oborech.  
Můžeme si díky němu vyzkoušet celý proces tvorby map — od načtení dat, přes jejich zpracování a analýzu až po finální kartografický výstup.  

<!-- 3 obrázky vedle sebe s mezerami, responsivní -->
<div style="display:flex; gap:12px; align-items:flex-start; justify-content:center; flex-wrap:wrap;">
  <figure style="margin:0; flex:1 1 280px; max-width:600px;">
    <img src="../assets/index/qgis1.jpg" style="width:100%; height:auto; display:block;" loading="lazy">
  </figure>
  <figure style="margin:0; flex:1 1 280px; max-width:600px;">
    <img src="../assets/index/qgis2.jpg" style="width:100%; height:auto; display:block;" loading="lazy">
  </figure>
  <figure style="margin:0; flex:1 1 280px; max-width:600px;">
    <img src="../assets/index/qgis3.jpg" style="width:100%; height:auto; display:block;" loading="lazy">
  </figure>
</div>





