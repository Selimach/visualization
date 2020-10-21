Mobilite\_RATP
================
Selim Ach
18/10/2020

Ce document est rédigé à des fins d’illustration et l’analyse se base
sur des données publiques provenant de la RATP. L’analyse statistique
est faite avec le logiciel de programmation R, et a pour but de donner
un aperçu des différentes possibilités de traitement de données, de
production d’indicateurs et autres graphiques.

-----

Source - <https://dataratp2.opendatasoft.com/explore/?sort=modified>

Ce jeu de données détaille le trafic des entrants directs sur le réseau
ferré RATP en 2019.

Les « entrants directs » sont exclusivement les voyageurs provenant de
la voie publique ou du réseau SNCF entrant sur le réseau de transport
RATP en validant un titre de transport valide.

Les voyageurs en correspondance (y compris correspondances métro/RER)
sur le réseau RATP ne sont pas comptabilisés.

### Statistiques descriptives générales

#### Fréquentation

![](Mobilite_RATP_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

#### Moyenne, fréquentation maximale et minimale

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:left;">

Réseau

</th>

<th style="text-align:right;">

Moyenne

</th>

<th style="text-align:right;">

Max

</th>

<th style="text-align:right;">

Min

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

Métro

</td>

<td style="text-align:right;">

4,593,587

</td>

<td style="text-align:right;">

51,141,374

</td>

<td style="text-align:right;">

169,939

</td>

</tr>

<tr>

<td style="text-align:left;">

RER

</td>

<td style="text-align:right;">

6,046,202

</td>

<td style="text-align:right;">

47,417,703

</td>

<td style="text-align:right;">

419,294

</td>

</tr>

</tbody>

</table>

### Statistiques descriptives par ligne de métro et RER

#### Pic voyageurs - RER

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:left;">

Réseau

</th>

<th style="text-align:left;">

Station

</th>

<th style="text-align:right;">

Trafic

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

RER

</td>

<td style="text-align:left;">

GARE DU NORD-RER

</td>

<td style="text-align:right;">

47,417,703

</td>

</tr>

</tbody>

</table>

#### Pic voyageurs - Métro

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:left;">

Réseau

</th>

<th style="text-align:left;">

Station

</th>

<th style="text-align:right;">

Trafic

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

Métro

</td>

<td style="text-align:left;">

GARE DU
NORD

</td>

<td style="text-align:right;">

51,141,374

</td>

</tr>

</tbody>

</table>

### Répartition des voyageurs RER et Métro

![](Mobilite_RATP_files/figure-gfm/unnamed-chunk-7-1.png)<!-- -->

<!--html_preserve-->

<div id="htmlwidget-1e6038637b4b468dbfcd" class="leaflet html-widget" style="width:672px;height:480px;">

</div>

<script type="application/json" data-for="htmlwidget-1e6038637b4b468dbfcd">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[[48.8576918345942,48.84368046702,48.8810816657367,48.89303960645],[2.34798963852442,2.3735398017355,2.357748079238,2.23749223664],null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},null,null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[48.84368046702,48.89303960645],"lng":[2.23749223664,2.3735398017355]}},"evals":[],"jsHooks":[]}</script>

<!--/html_preserve-->
