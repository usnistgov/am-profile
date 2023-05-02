# Additive Manufacturing Profile

This repository contains associated data for the manuscript *Data Assets and Risk Management for Additive Manufacturing* 
by [Fahad Milaat](https://www.nist.gov/people/fahad-milaat) and 
[Joshua Lubell](https://www.nist.gov/people/joshua-lubell). The associated data is the source 
of the [OSCAL](https://pages.nist.gov/OSCAL) representations in Section 4 of the manuscript. If you have not already read 
the manuscript, please read it now before reviewing the contents of this repository.

## Repository Contents

```src``` contains:
- ```csf-oscal-no-refs.xml```: an [XML](https://www.w3.org/XML/) representation of [Cybersecurity Framework](https://www.nist.gov/cyberframework) subcategory ID.AM-3 (omitting 
    informative references) in OSCAL [catalog](https://pages.nist.gov/OSCAL/concepts/layer/control/catalog/) 
    format.
- XML representations in OSCAL [profile](https://pages.nist.gov/OSCAL/concepts/layer/control/profile/) format.
    ```csf-oscal-profile-ot-id.am-3.xml``` supplements ID.AM-3 with guidance from the 
    [Guide to Operational Technology Security](https://csrc.nist.gov/publications/detail/sp/800-82/rev-3/draft). 
    ```csf-oscal-profile-additive-id.am-3.xml``` adds a additional layer of Additive Manufacturing security guidance to ID.AM-3. 

```resolved``` contains XML representations of ```csf-oscal-profile-ot-id.am-3.xml``` and ```csf-oscal-profile-additive-id.am-3.xml```
after applying OSCAL's 
[profile resolution algorithm](https://pages.nist.gov/OSCAL/concepts/processing/profile-resolution/). Profile resolution 
transforms an OSCAL profile into a "resolved" OSCAL catalog.

```json``` contains the contents of `src` and `resolved` converted into [JSON](https://www.json.org/) via OSCAL's 
[XML-to-JSON converters](https://github.com/usnistgov/OSCAL/tree/main/json). 

```yaml``` contains the contents of `json` converted into [YAML](https://yaml.org/) via a third-party JSON-to-YAML converter.
Since JSON is a subset of YAML, conversion from JSON to YAML is easy.

`css` contains a [Cascading Style Sheet](https://www.w3.org/Style/CSS/) for rendering the XML content in an XML authoring tool 
that supports CSS.