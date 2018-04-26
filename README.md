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

Maven build requires cheese-maven-plugin from https://github.com/davidedmonds/cheese-maven-plugin to be installed locally.
This is in order to generate a class with static members for each Cheese.
