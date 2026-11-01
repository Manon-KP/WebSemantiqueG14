# Lieux de tournage à Paris

Jeu de données sur les lieux de tournage à Paris

## Fichiers

* `lieux-de-tournage-a-paris.csv` : jeu de données téléchargé [ici](https://opendata.paris.fr/explore/dataset/lieux-de-tournage-a-paris/)
* `tournages.ttl` : le jeu de données au format RDF Turtle
* `construct.sparql` : requête SPARQL CONSTRUCT (Tarql) qui transforme le CSV en RDF
* `requetes.sparql` : nos requêtes SPARQL

## Conversion

```
tarql --delimiter ";" --no-header-row construct.sparql lieux-de-tournage-a-paris.csv > tournages.ttl
```

## Vocabulaires utilisés

schema.org, FOAF, WGS84 geo, Dublin Core