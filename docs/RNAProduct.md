---
parent: Entities
title: biolink:RNAProduct
grand_parent: Classes
layout: default
---

# Class: RNAProduct




URI: [biolink:RNAProduct](https://w3id.org/biolink/vocab/RNAProduct)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[OrganismTaxon],[NoncodingRNAProduct],[NamedThing],[GeneProduct],[Attribute],[Agent],[RNAProductIsoform],[RNAProduct%7Csynonym(i):label_type%20%2A;xref(i):iri_type%20%2A;name(i):symbol_type%20%3F;has_biological_sequence(i):biological_sequence%20%3F;id(i):string;iri(i):iri_type%20%3F;type(i):string%20%3F;description(i):narrative_text%20%3F;source(i):label_type%20%3F]%5E-[NoncodingRNAProduct],[RNAProduct]%5E-[RNAProductIsoform],[GeneProduct]%5E-[RNAProduct])

---


## Identifier prefixes

 * RNACENTRAL

## Parents

 *  is_a: [GeneProduct](GeneProduct.md) - The functional molecular product of a single gene. Gene products are either proteins or functional RNA molecules

## Children

 * [RNAProductIsoform](RNAProductIsoform.md) - Represents a protein that is a specific isoform of the canonical or reference RNA
 * [NoncodingRNAProduct](NoncodingRNAProduct.md)

## Referenced by class


## Attributes


### Inherited from entity:

 * [id](id.md)  <sub>REQ</sub>
    * Description: A unique identifier for a resource. Must be either a CURIE shorthand for a URI or a complete URI
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [iri](iri.md)  <sub>OPT</sub>
    * Description: An IRI for an entity. This is determined by the id using expansion rules.
    * range: [IriType](types/IriType.md)
    * in subsets: (translator_minimal,samples)
 * [type](type.md)  <sub>OPT</sub>
    * range: [String](types/String.md)
 * [name](name.md)  <sub>OPT</sub>
    * Description: A human-readable name for a thing
    * range: [LabelType](types/LabelType.md)
    * in subsets: (translator_minimal,samples)
 * [description](description.md)  <sub>OPT</sub>
    * Description: a human-readable description of a thing
    * range: [NarrativeText](types/NarrativeText.md)
    * in subsets: (translator_minimal)
 * [source](source.md)  <sub>OPT</sub>
    * Description: a lightweight analog to the association class 'has provider' slot, which is the string name, or the authoritative (i.e. database) namespace, designating the origin of the entity to which the slot belongs.
    * range: [LabelType](types/LabelType.md)
    * in subsets: (translator_minimal)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Agent](Agent.md)

### Inherited from genomic entity:

 * [has biological sequence](has_biological_sequence.md)  <sub>OPT</sub>
    * Description: connects a genomic feature to its sequence
    * range: [BiologicalSequence](types/BiologicalSequence.md)

### Inherited from macromolecular machine:

 * [macromolecular machine➞name](macromolecular_machine_name.md)  <sub>OPT</sub>
    * Description: genes are typically designated by a short symbol and a full name. We map the symbol to the default display name and use an additional slot for full name
    * range: [SymbolType](types/SymbolType.md)

### Inherited from material sample:

 * [has attribute](has_attribute.md)  <sub>0..*</sub>
    * Description: connects any named thing to an attribute
    * range: [Attribute](Attribute.md)
    * in subsets: (samples)

### Inherited from named thing:

 * [named thing➞category](named_thing_category.md)  <sub>1..*</sub>
    * range: [NamedThing](NamedThing.md)

### Inherited from thing with taxon:

 * [in taxon](in_taxon.md)  <sub>0..*</sub>
    * Description: connects a thing to a class representing a taxon
    * range: [OrganismTaxon](OrganismTaxon.md)
    * in subsets: (translator_minimal)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Exact Mappings:** | | CHEBI:33697 |
|  | | WIKIDATA:Q11053 |
