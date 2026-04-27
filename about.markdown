---
layout: default
title: About
permalink: /about/
---

# About Inscript

This project is an experimental database and converter designed to transform epigraphic data from Wikidata into TEI XML. The intended workflow consists of extracting items from Wikidata, converting them into TEI XML format, and subsequently uploading them to the Epigraphic Archive and make them searchable as well.

At present, the archive only contains a set of mock inscriptions, and is therefore not yet functional as a research tool. The next step is to establish a reliable method for accessing Wikidata (e.g. via API or SPARQL queries), which will enable the implementation of the data retrieval process.

## Points to consider

- how to access Wikidata (API vs SPARQL queries)
- how to structure and store inscriptions in TEI XML (possibly reusing the schema adopted for the mock data)
- how to manage Wikidata qualifiers (e.g. dates, measurements, and other contextual metadata)
