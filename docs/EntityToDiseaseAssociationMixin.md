---
parent: Class Mixins
title: biolink:EntityToDiseaseAssociationMixin
grand_parent: Classes
layout: default
---

# Class: EntityToDiseaseAssociationMixin


mixin class for any association whose object (target node) is a disease

URI: [biolink:EntityToDiseaseAssociationMixin](https://w3id.org/biolink/vocab/EntityToDiseaseAssociationMixin)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[SeverityValue],[Onset],[EntityToFeatureOrDiseaseQualifiersMixin],[Disease]%3Cobject%201..1-%20[EntityToDiseaseAssociationMixin%7Cfrequency_qualifier(i):frequency_value%20%3F],[VariantToDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[VariantAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[OrganismalEntityAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[GenotypeToDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[GenotypeAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[GeneToDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[GeneAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[CellLineAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociationMixin],[EntityToFeatureOrDiseaseQualifiersMixin]%5E-[EntityToDiseaseAssociationMixin],[VariantToDiseaseAssociation],[VariantAsAModelOfDiseaseAssociation],[OrganismalEntityAsAModelOfDiseaseAssociation],[GenotypeToDiseaseAssociation],[GenotypeAsAModelOfDiseaseAssociation],[GeneToDiseaseAssociation],[GeneAsAModelOfDiseaseAssociation],[Disease],[CellLineAsAModelOfDiseaseAssociation])

---


## Parents

 *  is_a: [EntityToFeatureOrDiseaseQualifiersMixin](EntityToFeatureOrDiseaseQualifiersMixin.md) - Qualifiers for entity to disease or phenotype associations.

## Mixin for

 * [CellLineAsAModelOfDiseaseAssociation](CellLineAsAModelOfDiseaseAssociation.md) (mixin) 
 * [GeneAsAModelOfDiseaseAssociation](GeneAsAModelOfDiseaseAssociation.md) (mixin) 
 * [GeneToDiseaseAssociation](GeneToDiseaseAssociation.md) (mixin) 
 * [GenotypeAsAModelOfDiseaseAssociation](GenotypeAsAModelOfDiseaseAssociation.md) (mixin) 
 * [GenotypeToDiseaseAssociation](GenotypeToDiseaseAssociation.md) (mixin) 
 * [OrganismalEntityAsAModelOfDiseaseAssociation](OrganismalEntityAsAModelOfDiseaseAssociation.md) (mixin) 
 * [VariantAsAModelOfDiseaseAssociation](VariantAsAModelOfDiseaseAssociation.md) (mixin) 
 * [VariantToDiseaseAssociation](VariantToDiseaseAssociation.md) (mixin) 

## Referenced by class


## Attributes


### Own

 * [entity to disease association mixin➞object](entity_to_disease_association_mixin_object.md)  <sub>REQ</sub>
     * Description: disease
     * Range: [Disease](Disease.md)
     * Example: MONDO:0020066 Ehlers-Danlos syndrome

### Inherited from entity to feature or disease qualifiers mixin:

 * [severity qualifier](severity_qualifier.md)  <sub>OPT</sub>
     * Description: a qualifier used in a phenotypic association to state how severe the phenotype is in the subject
     * Range: [SeverityValue](SeverityValue.md)
 * [onset qualifier](onset_qualifier.md)  <sub>OPT</sub>
     * Description: a qualifier used in a phenotypic association to state when the phenotype appears is in the subject
     * Range: [Onset](Onset.md)

### Inherited from frequency qualifier mixin:

 * [frequency qualifier](frequency_qualifier.md)  <sub>OPT</sub>
     * Description: a qualifier used in a phenotypic association to state how frequent the phenotype is observed in the subject
     * Range: [FrequencyValue](types/FrequencyValue.md)

### Domain for slot:

 * [entity to disease association mixin➞object](entity_to_disease_association_mixin_object.md)  <sub>REQ</sub>
     * Description: disease
     * Range: [Disease](Disease.md)
     * Example: MONDO:0020066 Ehlers-Danlos syndrome