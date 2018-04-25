Cheese List
===========

A list of cheeses, extracted from Wikipedia using https://query.wikidata.org and the SPARQL:

```sparql
#Cheeses
SELECT ?itemLabel WHERE {
  ?item wdt:P279 wd:Q10943.
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
}
```

Built as a JAR for JVM languages, and as a Node module for JS.