---
parent: Associations
title: biolink:ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation
grand_parent: Classes
layout: default
---

# Class: ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation


A regulatory relationship between two genes

URI: [biolink:ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation](https://w3id.org/biolink/vocab/ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation)


---

![img](https://yuml.me/diagram/nofunky;dir:TB/class/[RetrievalSource],[Publication],[OntologyClass],[InformationResource],[GeneOrGeneProduct],[EvidenceType],[GeneOrGeneProduct]%3Cobject%201..1-++[ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation%7Cobject_direction_qualifier:DirectionQualifierEnum%20%3F;predicate:predicate_type;negated(i):boolean%20%3F;timepoint(i):time_type%20%3F;original_subject(i):string%20%3F;original_predicate(i):uriorcurie%20%3F;original_object(i):string%20%3F;subject_closure(i):string%20%2A;object_closure(i):string%20%2A;subject_namespace(i):string%20%3F;object_namespace(i):string%20%3F;subject_label_closure(i):string%20%2A;object_label_closure(i):string%20%2A;type(i):string%20%2A;category(i):category_type%20%2A;id(i):string;iri(i):iri_type%20%3F;name(i):label_type%20%3F;description(i):narrative_text%20%3F],[ChemicalEntityOrGeneOrGeneProduct]%3Csubject%201..1-++[ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation],[Association]%5E-[ChemicalEntityOrGeneOrGeneProductRegulatesGeneAssociation],[ChemicalEntityOrGeneOrGeneProduct],[Attribute],[Association])

---


## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Referenced by class


## Attributes


### Own

 * [object](object.md)  <sub>1..1</sub>
     * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)
 * [object direction qualifier](object_direction_qualifier.md)  <sub>0..1</sub>
     * Range: [DirectionQualifierEnum](DirectionQualifierEnum.md)
     * in subsets: (translator_minimal)
 * [predicate](predicate.md)  <sub>1..1</sub>
     * Description: A high-level grouping for the relationship type. AKA minimal predicate. This is analogous to category for nodes.
     * Range: [PredicateType](types/PredicateType.md)
 * [subject](subject.md)  <sub>1..1</sub>
     * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)

### Inherited from association:

 * [subject](subject.md)  <sub>1..1</sub>
     * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)
 * [predicate](predicate.md)  <sub>1..1</sub>
     * Description: A high-level grouping for the relationship type. AKA minimal predicate. This is analogous to category for nodes.
     * Range: [PredicateType](types/PredicateType.md)
 * [object](object.md)  <sub>1..1</sub>
     * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)
 * [negated](negated.md)  <sub>0..1</sub>
     * Description: if set to true, then the association is negated i.e. is not true
     * Range: [Boolean](types/Boolean.md)
 * [qualifiers](qualifiers.md)  <sub>0..\*</sub>
     * Description: connects an association to qualifiers that modify or qualify the meaning of that association
     * Range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..\*</sub>
     * Description: One or more publications that report the statement expressed in an  Association, or provide information used as evidence supporting this statement.
     * Range: [Publication](Publication.md)
 * [has evidence](has_evidence.md)  <sub>0..\*</sub>
     * Description: connects an association to an instance of supporting evidence
     * Range: [EvidenceType](EvidenceType.md)
 * [knowledge source](knowledge_source.md)  <sub>0..1</sub>
     * Description: An Information Resource from which the knowledge expressed in an Association was retrieved, directly or indirectly. This can be any resource through which the knowledge passed on its way to its currently serialized form. In practice, implementers should use one of the more specific subtypes of this generic property.
     * Range: [InformationResource](InformationResource.md)
 * [primary knowledge source](primary_knowledge_source.md)  <sub>0..1</sub>
     * Description: The most upstream source of the knowledge expressed in an Association that an implementer can identify.  Performing a rigorous analysis of upstream data providers is expected; every effort is made to catalog the most upstream source of data in this property.  Only one data source should be declared primary in any association.  "aggregator knowledge source" can be used to capture non-primary sources.
     * Range: [InformationResource](InformationResource.md)
 * [aggregator knowledge source](aggregator_knowledge_source.md)  <sub>0..\*</sub>
     * Description: An intermediate aggregator resource from which knowledge expressed in an Association was retrieved downstream of the original source, on its path to its current serialized form.
     * Range: [InformationResource](InformationResource.md)
 * [timepoint](timepoint.md)  <sub>0..1</sub>
     * Description: a point in time
     * Range: [TimeType](types/TimeType.md)
 * [original subject](original_subject.md)  <sub>0..1</sub>
     * Description: used to hold the original subject of a relation (or predicate) that an external knowledge source uses before transformation to match the biolink-model specification.
     * Range: [String](types/String.md)
 * [original predicate](original_predicate.md)  <sub>0..1</sub>
     * Description: used to hold the original relation/predicate that an external knowledge source uses before transformation to match the biolink-model specification.
     * Range: [Uriorcurie](types/Uriorcurie.md)
 * [original object](original_object.md)  <sub>0..1</sub>
     * Description: used to hold the original object of a relation (or predicate) that an external knowledge source uses before transformation to match the biolink-model specification.
     * Range: [String](types/String.md)
 * [subject category](subject_category.md)  <sub>0..1</sub>
     * Description: Used to hold the biolink class/category of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [OntologyClass](OntologyClass.md)
     * Example: biolink:Gene The subject category of the association between the gene 'BRCA1' and the disease 'breast cancer' is 'biolink:Gene'.
 * [object category](object_category.md)  <sub>0..1</sub>
     * Description: Used to hold the biolink class/category of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [OntologyClass](OntologyClass.md)
     * Example: biolink:Disease The object category of the association between the gene 'BRCA1' and the disease 'breast cancer' is 'biolink:Disease'.
 * [subject closure](subject_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the subject closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
 * [object closure](object_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the object closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
     * Example: ['MONDO:0000167', 'MONDO:0005395'] The object closure of the association between the gene 'BRCA1' and the disease 'breast cancer' is the set of all diseases that are ancestors of 'breast cancer' in the MONDO ontology.  Note: typically the "subclass of" and "part of"  relations are used to construct the closure, but other relations may be used as well.
 * [subject category closure](subject_category_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the subject category closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [OntologyClass](OntologyClass.md)
     * Example: ['biolink:Gene", "biolink:NamedThing'] The subject category closure of the association between the gene 'BRCA1' and the disease 'breast cancer' is the set of all biolink classes that are ancestors of 'biolink:Gene' in the biolink model.  Note: typically the "subclass of" and "part of"  relations are used to construct the closure, but other relations may be used as well.
 * [object category closure](object_category_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the object category closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [OntologyClass](OntologyClass.md)
     * Example: ['biolink:Disease", "biolink:NamedThing'] The object category closure of the association between the gene 'BRCA1' and the disease 'breast cancer' is the set of all biolink classes that are ancestors of 'biolink:Disease' in the biolink model.  Note: typically the "subclass of" and "part of"  relations are used to construct the closure, but other relations may be used as well.
 * [subject namespace](subject_namespace.md)  <sub>0..1</sub>
     * Description: Used to hold the subject namespace of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
     * Example: NCBIGene The subject namespace of the association between the gene 'BRCA1' and the disease 'breast cancer' is 'NCBIGene'.
 * [object namespace](object_namespace.md)  <sub>0..1</sub>
     * Description: Used to hold the object namespace of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
     * Example: MONDO The object namespace of the association between the gene 'BRCA1' and the disease 'breast cancer' is 'MONDO'.
 * [subject label closure](subject_label_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the subject label closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
     * Example: ['BRACA1'] The subject label closure of the association between the gene 'BRCA1' and the disease 'breast cancer' is the set of all labels that are ancestors of 'BRCA1' in the biolink model.
 * [object label closure](object_label_closure.md)  <sub>0..\*</sub>
     * Description: Used to hold the object label closure of an association. This is a denormalized  field used primarily in the SQL serialization of a knowledge graph via KGX.
     * Range: [String](types/String.md)
     * Example: ['breast cancer', 'cancer'] The object label closure of the association between the gene 'BRCA1' and the disease 'breast cancer' is the set of all labels that are ancestors of 'breast cancer' in the biolink model.
 * [retrieval source ids](retrieval_source_ids.md)  <sub>0..\*</sub>
     * Description: A list of retrieval sources that served as a source of knowledge expressed in an Edge, or a source of data used to generate this knowledge.
     * Range: [RetrievalSource](RetrievalSource.md)
     * in subsets: (translator_minimal)
 * [type](type.md)  <sub>0..\*</sub>
     * Range: [String](types/String.md)
 * [category](category.md)  <sub>0..\*</sub>
     * Description: Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class.
 * In a neo4j database this MAY correspond to the neo4j label tag.
 * In an RDF database it should be a biolink model class URI.
This field is multi-valued. It should include values for ancestors of the biolink class; for example, a protein such as Shh would have category values `biolink:Protein`, `biolink:GeneProduct`, `biolink:MolecularEntity`, ...
In an RDF database, nodes will typically have an rdf:type triples. This can be to the most specific biolink class, or potentially to a class more specific than something in biolink. For example, a sequence feature `f` may have a rdf:type assertion to a SO class such as TF_binding_site, which is more specific than anything in biolink. Here we would have categories {biolink:GenomicEntity, biolink:MolecularEntity, biolink:NamedThing}
     * Range: [CategoryType](types/CategoryType.md)
     * in subsets: (translator_minimal)

### Inherited from entity:

 * [iri](iri.md)  <sub>0..1</sub>
     * Description: An IRI for an entity. This is determined by the id using expansion rules.
     * Range: [IriType](types/IriType.md)
     * in subsets: (translator_minimal,samples)
 * [category](category.md)  <sub>0..\*</sub>
     * Description: Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class.
 * In a neo4j database this MAY correspond to the neo4j label tag.
 * In an RDF database it should be a biolink model class URI.
This field is multi-valued. It should include values for ancestors of the biolink class; for example, a protein such as Shh would have category values `biolink:Protein`, `biolink:GeneProduct`, `biolink:MolecularEntity`, ...
In an RDF database, nodes will typically have an rdf:type triples. This can be to the most specific biolink class, or potentially to a class more specific than something in biolink. For example, a sequence feature `f` may have a rdf:type assertion to a SO class such as TF_binding_site, which is more specific than anything in biolink. Here we would have categories {biolink:GenomicEntity, biolink:MolecularEntity, biolink:NamedThing}
     * Range: [CategoryType](types/CategoryType.md)
     * in subsets: (translator_minimal)
 * [type](type.md)  <sub>0..\*</sub>
     * Range: [String](types/String.md)
 * [has attribute](has_attribute.md)  <sub>0..\*</sub>
     * Description: connects any entity to an attribute
     * Range: [Attribute](Attribute.md)
     * in subsets: (samples)

### Inherited from information resource:

 * [information resource status](information_resource_status.md)  <sub>0..1</sub>
     * Description: the status of the infores identifier, default is released
     * Range: [InformationResourceStatusEnum](InformationResourceStatusEnum.md)
 * [id](id.md)  <sub>1..1</sub>
     * Description: A unique identifier for an entity. Must be either a CURIE shorthand for a URI or a complete URI
     * Range: [String](types/String.md)
     * in subsets: (translator_minimal)
 * [description](description.md)  <sub>0..1</sub>
     * Description: a human-readable description of an entity
     * Range: [NarrativeText](types/NarrativeText.md)
     * in subsets: (translator_minimal)

### Inherited from macromolecular machine mixin:

 * [name](name.md)  <sub>0..1</sub>
     * Description: A human-readable name for an attribute or entity.
     * Range: [LabelType](types/LabelType.md)
     * in subsets: (translator_minimal,samples)

### Domain for slot:

 * [object](object.md)  <sub>1..1</sub>
     * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)
 * [object direction qualifier](object_direction_qualifier.md)  <sub>0..1</sub>
     * Range: [DirectionQualifierEnum](DirectionQualifierEnum.md)
     * in subsets: (translator_minimal)
 * [predicate](predicate.md)  <sub>1..1</sub>
     * Description: A high-level grouping for the relationship type. AKA minimal predicate. This is analogous to category for nodes.
     * Range: [PredicateType](types/PredicateType.md)
 * [subject](subject.md)  <sub>1..1</sub>
     * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
     * Range: [NamedThing](NamedThing.md)