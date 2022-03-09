## Use case
A general use case of the PKG ontology is in the context of collaborative searching as learning scenarios. More and more often, students use search engines to learn more 
about a specific subject. However, the large number of documents provided as search results constitutes an obstacle. Students have to read, understand, analyse all the 
results. Search engines support their users in performing keyword-based searches, but they do not provide functionalities specifically designed to facilitate students' 
searches for learning tasks [^1]. Moreover, the collaboration between users is not enabled, hindering the possibility of implementing project-based learning or 
team-based learning activities. The PKG ontology can facilitate collaborative search and collaborative learning by creating Personal Knowledge Graphs in the backend 
of a system application. 

In particular, a specific use case of the PKG ontology has been integrated within the Learnweb e-learning platform[^2][^3].
Learnweb is a platform supporting collaborative searching and learning, and our ontology assists the integration of a new visualisation interface[^4].
In the backend of the application, the *SearchSession* related classes are integrated via the classical search interface of Learnweb, and the
*InputStream* is created. Then the stream is passed to the DBpedia Spotlight[^5] software, which generates the *RecognizedEntities*
from the DBpedia Knowledge Graph. This output is then processed together with the data gathered during the user's activity, and the *SharedObject*
is produced concerning *Accessibility* parameters. Finally, this object is shared with the Learnweb user interface, in which the summary of the users'
actions during a collaborative search activity is shown. Based on the algorithmic analysis, the display shows the most important entities that members are
searching for related to the learning project they are collaborating on. The display is in graph form, with the nodes representing the core concepts of the
search results and the edges showing how they are interconnected. 

[^1]: Ceroni, A., Gadiraju, U.K., Fisichella, M.: Improving event detection by automatically assessing validity of event occurrence in text. In: Proceedings of the 24th 
ACM International Conference on Information and Knowledge Management, CIKM 2015, Melbourne, VIC, Australia, October 19 - 23, 2015. pp. 1815–1818. ACM (2015)
[^2]: Marenzi, I., Zerr, S.: Multiliteracies and active learning in CLIL - the development of learnweb2.0. IEEE Trans. Learn. Technol. 5(4), 336–348 (2012).
https://doi.org/10.1109/TLT.2012.14, https://doi.org/10.1109/TLT.2012.14
[^3]: Tolmachova, T., Ilkou, E., Xu, L.: Working towards the ideal search history interface. In: Proceedings of the CIKM 2020 Workshops co-located with 29th ACM
International Conference on Information and Knowledge Management (CIKM 2020), Galway, Ireland, October 19-23, 2020. CEUR-WS.org (2020)
[^4]: lkou, E., Tolmachova, T., Fisichella, M., Taibi, D.: Collabgraph: A graph-based collaborative search summary visualisation (2022)
[^5]: Mendes, P.N., Jakob, M., García-Silva, A., Bizer, C.: Dbpedia spotlight: shedding light on the web of documents. In: Proceedings of the 7th international conference
on semantic systems. pp. 1–8 (2011)
