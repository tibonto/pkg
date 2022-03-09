## PKG ontology description

PKG ontology is proposed to create personal knowledge graphs for web search. It was implemented in OWL using the Protégé editor. This resource fills the need 
for semantic representation of the user's profile and data related search activity under a unified framework that accommodates associations between entities and attributes.
Our ontology introduces the necessary classes and properties to construct a Personal Knowledge Graph on a web search environment. 

PKG ontology extends on the EduCOR (educor) ontology[^1] and reuses syntax for its classes and properties from schema.org[^2] (schema), and friend of a friend vocabulary[^3] 
(foaf), as can be seen in the Table:
| Syntax  | Description |
|  :----  |    :----    |
| base    | https://github.com/tibonto/pkg/       |
| educor  | https://github.com/tibonto/educor\#   |
| schema  | https://schema.org/   |
| foaf    | http://xmlns.com/foaf/spec/   |


Our ontology is aligned with FAIR principles[^4]. Our data and metadata are assigned globally unique and persistent identifiers and clearly and explicitly include the
identifier of the data they describe. They are described in rich metadata, and we reuse vocabularies that follow FAIR principles and include qualified references to them.
Our ontology can be found in the TIBonto registry[^5], which also offers the full documentation and visualisation of the ontology. The ontology data can be retrieved 
from there via the querying API. 
Also, we describe the scope of our data and have them published under the licence CC BY-SA 4.0, and our ontology has the canonical citation 
``E. Ilkou et al: Personal Knowledge Graph Ontology for Web Search. March 2022. https://github.com/tibonto/pkg''.

The main class in our ontology is the *SearchSession* as it is also highlighted in the Figure:

![PKG ontology](https://github.com/tibonto/pkg/raw/gh-pages/Pkgonto.png)

Together with the classes *UserProfile*, and *Group* they create the *InputStream* for the computational algorithm that will perform the semantic annotation. The ontology can be used to 
create a Personal Knowledge Graph and enhance semantically a back end of a web search application, when linking to knowledge graphs. That can happen via the 
*RecognizedEntites* which returns the output result of the computation of the connection with Linked Open Data resources. The result is the recognized entities 
from the connected knowledge graph together with their confidence score based on the named entity recognition software that is utilised. Finally, the *SharedObject* 
shares the items needed for the downstream application related to search activity with respect to user's privacy and accessibility rights from the *Accessibility* class.

[^1]: Ilkou, E., Abu-Rasheed, H., Tavakoli, M., Hakimov, S., Kismihók, G., Auer, S., Nejdl, W.: Educor: An educational and career-oriented recommendation ontology.
In: International Semantic Web Conference. pp. 546–562. Springer (2021)
[^2]: https://schema.org/
[^3]: http://xmlns.com/foaf/spec/
[^4]: Wilkinson, M.D., Dumontier, M., Aalbersberg, I.J., Appleton, G., Axton, M., Baak, A., Blomberg, N., Boiten, J.W., da Silva Santos, L.B., Bourne, P.E., et al.: The fair
guiding principles for scientific data management and stewardship. Scientific data 3(1), 1–9 (2016)
[^5]: The ontology page can be found in http://ontology.tib.eu/pkg/
