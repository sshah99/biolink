---
parent: Classes
title: biolink:VariantToPopulationAssociation
grand_parent: Browse Biolink Model
layout: default
---

# Type: VariantToPopulationAssociation


An association between a variant and a population, where the variant has particular frequency in the population

URI: [biolink:VariantToPopulationAssociation](https://w3id.org/biolink/vocab/VariantToPopulationAssociation)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[VariantToThingAssociation],[PopulationOfIndividualOrganisms]%3Cobject%201..1-%20[VariantToPopulationAssociation|has_count:integer%20%3F;has_total:integer%20%3F;has_quotient:double%20%3F;has_percentage:double%20%3F;relation(i):uriorcurie;id(i):string;negated(i):boolean%20%3F],[SequenceVariant]%3Csubject%201..1-%20[VariantToPopulationAssociation],[VariantToPopulationAssociation]uses%20-.-%3E[VariantToThingAssociation],[VariantToPopulationAssociation]uses%20-.-%3E[FrequencyQuantifier],[VariantToPopulationAssociation]uses%20-.-%3E[FrequencyQualifierMixin],[Association]%5E-[VariantToPopulationAssociation],[SequenceVariant],[Publication],[Provider],[PopulationOfIndividualOrganisms],[OntologyClass],[FrequencyValue],[FrequencyQuantifier],[FrequencyQualifierMixin],[Association])

---


## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Uses Mixins

 *  mixin: [VariantToThingAssociation](VariantToThingAssociation.md)
 *  mixin: [FrequencyQuantifier](FrequencyQuantifier.md)
 *  mixin: [FrequencyQualifierMixin](FrequencyQualifierMixin.md) - Qualifier for frequency type associations

## Referenced by class


## Attributes


### Own

 * [variant to population association➞has count](variant_to_population_association_has_count.md)  <sub>OPT</sub>
    * range: [Integer](types/Integer.md)
 * [variant to population association➞has quotient](variant_to_population_association_has_quotient.md)  <sub>OPT</sub>
    * range: [Double](types/Double.md)
 * [variant to population association➞has total](variant_to_population_association_has_total.md)  <sub>OPT</sub>
    * range: [Integer](types/Integer.md)
 * [variant to population association➞object](variant_to_population_association_object.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)
 * [variant to population association➞subject](variant_to_population_association_subject.md)  <sub>REQ</sub>
    * range: [SequenceVariant](SequenceVariant.md)

### Inherited from association:

 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: The relation which describes an association between a subject and an object in a more granular manner. Usually this is a term from Relation Ontology, but it can be any edge CURIE.
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [association➞id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](types/Boolean.md)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Provider](Provider.md)

### Inherited from frequency qualifier mixin:

 * [frequency qualifier](frequency_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state how frequent the phenotype is observed in the subject
    * range: [FrequencyValue](FrequencyValue.md)

### Inherited from frequency quantifier:

 * [has count](has_count.md)  <sub>OPT</sub>
    * Description: number of things with a particular property
    * range: [Integer](types/Integer.md)
 * [has total](has_total.md)  <sub>OPT</sub>
    * Description: total number of things in a particular reference set
    * range: [Integer](types/Integer.md)
 * [has quotient](has_quotient.md)  <sub>OPT</sub>
    * range: [Double](types/Double.md)
 * [has percentage](has_percentage.md)  <sub>OPT</sub>
    * Description: equivalent to has quotient multiplied by 100
    * range: [Double](types/Double.md)

### Domain for slot:

 * [variant to population association➞has count](variant_to_population_association_has_count.md)  <sub>OPT</sub>
    * range: [Integer](types/Integer.md)
 * [variant to population association➞has quotient](variant_to_population_association_has_quotient.md)  <sub>OPT</sub>
    * range: [Double](types/Double.md)
 * [variant to population association➞has total](variant_to_population_association_has_total.md)  <sub>OPT</sub>
    * range: [Integer](types/Integer.md)
 * [variant to population association➞object](variant_to_population_association_object.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)
 * [variant to population association➞subject](variant_to_population_association_subject.md)  <sub>REQ</sub>
    * range: [SequenceVariant](SequenceVariant.md)