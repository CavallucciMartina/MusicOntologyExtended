# MusicOntologyExtended
Extension of [Music Ontology (MO)](http://musicontology.com/)

This project refers to a personal project of Semantic Web Course at University.

## Exstension
### OWL/RDFS
* Class Instrument Taxonomy
* Instrument as Individuals
* Class Concert as subclass of Performance
* Class Location of Concert
* Musical Genre as Individuals
* Concert Vendor as Individuals
* Concert Ticket as Individuals

The object properties and data properties referring to the above objects have also been implemented. 

### SPARQL
The following queries have been implemented:
* Concerts with sold out seats
* Mumber of artists in the Band
* Most expensive concert tickets of 2021 in USA
* Seller who has sold more tickets in Italy 

### SWRL
The following inference rules have been implemented:
* ``` instrument (?perf , ?inst) ^ performed (?ag , ?perf) ->hasInstrumentSkill (?ag , ?inst) ```
* ``` hasGenre (?perf , ?gen) ^ performed (?ag, ?perf) -> WorkGenre (?ag, ?gen) ```
* ``` Event(?perf) ^ NumberSeat (?perf , ?seat) ^ MaxTicket (?perf , ?seat) ->hasFullTicket (?perf , ?perf) ```

### Documentation
The project report is in: WS-MusicOntology-report.pdf