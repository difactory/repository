[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

# Digital Factory Repository

This repository contains [**data sets**](#data-sets) related to digital factory applications, including:

- [3D models](models/) of assets in [VR-compatible format](https://virtualfactory.gitbook.io/vlft/kb/instantiation/3d-models) (e.g. .glb, .gltf, .obj)
- [scene configuration](scenes/) of production systems, labs defined according to a [JSON schema](https://virtualfactory.gitbook.io/vlft/kb/instantiation/assets/json)
- [spreadsheets](/spreadsheets/) defining the configuration of production systems, labs according to a [template](https://virtualfactory.gitbook.io/vlft/kb/instantiation/assets/spreadsheet)
- [ontologies](ontoeng/), both T-box (cf. [Factory Data Model](https://virtualfactory.gitbook.io/vlft/kb/fdm)) and [A-box](https://virtualfactory.gitbook.io/vlft/kb/instantiation/assets/ontology) modules
- [SPARQL queries and updates](sparql/) customized to [access](https://virtualfactory.gitbook.io/vlft/kb/fdm/sparql-queries) and [modify](https://virtualfactory.gitbook.io/vlft/kb/fdm/sparql-updates) the [ontologies](ontoeng/)
- [animations](animations/) defining the dynamic behaviour of scene configurations according to a [JSON schema](https://virtualfactory.gitbook.io/vlft/kb/instantiation/animations)

The VLFT (Virtual Learning Factory Toolkit) [gitbook](https://virtualfactory.gitbook.io/vlft) provides an extended documentation.

Please check the [**references**](#references) for related publications.

## Data sets
The content of the folders is interlinked and can be grouped into demos, classworks, examples, etc.
In principle the data sets can be exploited by any software tools. However, they are already compatible with the following prototype tools:
- [VEB.js](https://virtualfactory.gitbook.io/vlft/tools/vebjs) (Virtual Environment based on Babylon.js), a reconfigurable model-driven virtual environment application based on [Babylon.js](https://www.babylonjs.com/), a complete JavaScript framework and graphics engine for building 3D applications with HTML5 and WebGL (Web Graphics Library) - ([live demo](https://difactory.github.io/DF/tools/VEBjs.html))
- [OntoGuiWeb](https://virtualfactory.gitbook.io/vlft/tools/ontoguiweb), a web application providing a graphical user interface for the instantiation and exploration of OWL ontologies - ([live demo](https://difactory.github.io/DF/tools/OntoGuiWeb.html))

The following table gives an overview of the available data for the various data sets:
- **Type**, i.e. type of use case, e.g. **demo** (demo of factory), **VL** (Virtual Lab), **CW** (Classwork), **UC** (Use Case), **ex** (example)
- **Doc**, i.e. link to the documentation of the use case
- **VR**, i.e. VR rendering using VEB.js
- **HiQ**, i.e. high-quality VR rendering using VEB.js
- **Scene**, i.e. definition of the use case in a JSON file
- **Onto**, i.e. definition of the use case in an ontology
- **3D**, i.e. 3D models of the use case
- **Anim**, i.e. animation of the use case
- **Table**, i.e. definition of the use case in spreadsheet table(s)


| Title                                                      | Type | Doc       | VR        | HiQ  | Scene    | Onto     | 3D       | Anim     | Table    |
|------------------------------------------------------------|------|-----------|-----------|----------|----------|----------|----------|----------|----------|
| Automated Assembly Line producing hinges                   | demo | [link](https://virtualfactory.gitbook.io/vlft/use-cases/assembly-line)  | [link](https://difactory.github.io/DF/scenes/VFLab/glb.html)  | [link](https://difactory.github.io/DF/scenes/VFLab/glbpbr.html) | [link](https://difactory.github.io/repository/scenes/demo/VFLab.json) | [link](https://difactory.github.io/repository/ontoeng/demo/VFLab.owl) | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine) | [link](https://difactory.github.io/repository/scenes/demo/VFLab_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/VF_UseCase_AssemblyLine.xlsx) |
| Automated Assembly Line producing hinges (reduced version) | demo |   |  [link](https://difactory.github.io/DF/scenes/DFAssemblyLine/glb.html) | [link](https://difactory.github.io/DF/scenes/DFAssemblyLine/glbpbr.html) | [link](https://difactory.github.io/repository/scenes/demo/DFAssemblyLine.json) | [link](https://difactory.github.io/repository/ontoeng/demo/DFAssemblyLine.owl) | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine) | [link](https://difactory.github.io/repository/scenes/demo/DFAssemblyLine_anim.json) |  |
| Production cell                                                         | demo |  |  [link](https://difactory.github.io/DF/scenes/DFProductionCell/glb.html) |  | [link](https://difactory.github.io/repository/scenes/demo/DFProductionCell.json) | [link](https://difactory.github.io/repository/ontoeng/demo/DFProductionCell.owl) | [link](https://github.com/difactory/repository/tree/main/models/ProdCell) |   |   |
|||||||||||
|  Production line     |  CW |   |  [link](https://difactory.github.io/DF/scenes/CW/ProductionLine.html) |  | [link](https://difactory.github.io/repository/scenes/CW/ProductionLine.json) | [link](https://difactory.github.io/repository/ontoeng/CW/ProductionLine.owl) | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine) | [link](https://difactory.github.io/repository/scenes/CW/ProductionLine_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/CwProductionLine.xlsx) |
|  Robotic cell      | CW  |    |  [link](https://difactory.github.io/DF/scenes/CW/RoboticCell.html) |   | [link](https://difactory.github.io/repository/scenes/CW/RoboticCell.json) | [link](https://difactory.github.io/repository/ontoeng/CW/RoboticCell.owl) | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine) | [link](https://difactory.github.io/repository/scenes/CW/RoboticCell_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/CwRoboticCell.xlsx) |
|||||||||||
|  PERFORM Lab          |  VL |  [link](https://github.com/difactory/DF/blob/main/docs/AVATAR-JLL/JLL_doc.md#1-perform-lab) |  [link](https://difactory.github.io/DF/scenes/VL/PERFORM_glb.html) |  | [link](https://difactory.github.io/repository/scenes/VL/PERFORM.json) | [link](https://difactory.github.io/repository/ontoeng/VL/PERFORM.ttl)  | [link](https://github.com/difactory/repository/tree/main/models/VL/PERFORM) | [link](https://difactory.github.io/repository/scenes/VL/PERFORM_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/VL_STIIMA_PERFORM.xlsx) |
|  RDM Lab          |  VL |  [link](https://link.springer.com/chapter/10.1007/978-3-319-94358-9_21#Sec8) |  [link](https://difactory.github.io/DF/scenes/VL/RdmPlant.html) |  | [link](https://difactory.github.io/repository/scenes/VL/RdmPlant.json) | [link](https://difactory.github.io/repository/ontoeng/VL/RdmPlant.ttl) | [link](https://github.com/difactory/repository/tree/main/models/VL/RDM) |  |  |
|||||||||||
| ControlPolicy01 | UC| | | | [link](https://difactory.github.io/repository/scenes/UC/ControlPolicy01.json) | [link](https://difactory.github.io/repository/ontoeng/UC/ControlPolicy01.ttl) |  |  | [link](https://difactory.github.io/repository/spreadsheets/UC_ControlPolicy01.xlsx) |
| PickPlaceCell | UC| | [link](https://difactory.github.io/DF/scenes/UC/PickPlaceCell.html)| | [link](https://difactory.github.io/repository/scenes/UC/PickPlaceCell.json) |  | [link](https://github.com/difactory/repository/tree/main/models/PickPlaceCell) |  |  |
|||||||||||
|  Example #1   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/assets-and-animations#example-1) |  [link](https://difactory.github.io/DF/scenes/ex/ex1.html) |  | [link](https://difactory.github.io/repository/scenes/ex/example_1.json) |  | [link](https://raw.githubusercontent.com/KhronosGroup/glTF-Sample-Models/master/2.0/WaterBottle/glTF-Binary/WaterBottle.glb) | [link](https://difactory.github.io/repository/scenes/ex/example_1_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/VF_assets_example1.xlsx) |
|  Example #2   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/assets-and-animations#example-2) |  [link](https://difactory.github.io/DF/scenes/ex/ex2.html) |  | [link](https://difactory.github.io/repository/scenes/ex/example_2.json) |  | [link](https://github.com/difactory/repository/tree/main/models/DemoFactory) | [link](https://difactory.github.io/repository/scenes/ex/example_2_anim.json) | [link](https://difactory.github.io/repository/spreadsheets/VF_assets_example2.xlsx) |
|  Example #3   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/assets-and-animations#example-3) |  [link](https://difactory.github.io/DF/scenes/ex/ex3.html) |  | [link](https://difactory.github.io/repository/scenes/ex/example_3.json) | | [link](https://github.com/difactory/repository/tree/main/models/DemoFactory) | [link](https://difactory.github.io/repository/scenes/ex/example_3_anim.json) | |
|  Product Example #1   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/factory-assets/assembled-product#scene-examples-hinge) |  [link](https://difactory.github.io/DF/scenes/ex/hinge1.html) |  | [link](https://difactory.github.io/repository/scenes/ex/HingeClones.json) |  | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine/GLB) |  | [link](https://difactory.github.io/repository/spreadsheets/ex_HingeClones.xlsx) |
|  Product Example #2   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/factory-assets/assembled-product#scene-2-customized-components-of-hinge) |  [link](https://difactory.github.io/DF/scenes/ex/hinge2.html) |  | [link](https://difactory.github.io/repository/scenes/ex/HingeCustomizedComponents.json) | | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine/GLB) | | [link](https://difactory.github.io/repository/spreadsheets/ex_HingeCustomizedComponents.xlsx) |
|  Product Example #3   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/factory-assets/assembled-product#scene-3-hidden-components-of-hinge) |  [link](https://difactory.github.io/DF/scenes/ex/hinge3.html) |  | [link](https://difactory.github.io/repository/scenes/ex/HingeHiddenComponents.json) |  | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine/GLB) |  | [link](https://difactory.github.io/repository/spreadsheets/ex_HingeHiddenComponents.xlsx) |
|  Machine Example   |  ex  |  [link](https://virtualfactory.gitbook.io/vlft/use-cases/factory-assets/workstation) |  [link](https://difactory.github.io/DF/scenes/ex/pi1.html) |  | [link](https://difactory.github.io/repository/scenes/ex/PIsClones.json) |  | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine/GLB) |  | [link](https://difactory.github.io/repository/spreadsheets/ex_PIsClones.xlsx) |
|  Physics Example   |  ex  |   |  [link](https://difactory.github.io/DF/scenes/ex/physics.html) |  | [link](https://difactory.github.io/repository/scenes/ex/Physics.json) |  | [link](https://github.com/difactory/repository/tree/main/models/AssemblyLine/GLB) |  | [link](https://difactory.github.io/repository/spreadsheets/ex_Physics.xlsx) |


## References

* Terkaj, W., Annoni, M., Martinez, B.O., Pessot, E., Sortino, M., Urgo, M., *2024*. **Digital Twin for Factories: Challenges and Industrial Applications**, in: Carrino, L., Galantucci, L.M., Settineri, L. (Eds.), Selected Topics in Manufacturing: Emerging Trends from the Perspective of AITeM’s Young Researchers, Lecture Notes in Mechanical Engineering. Springer Nature Switzerland, Cham, pp. 255–274. https://doi.org/10.1007/978-3-031-41163-2_13
* Berardinucci, F., Colombo, G., Lorusso, M., Manzini, M., Terkaj, W., Urgo, M., *2022*. **A learning workflow based on an integrated digital toolkit to support education in manufacturing system engineering**. Journal of Manufacturing Systems 63, 411–423. https://doi.org/10.1016/j.jmsy.2022.04.003
* Urgo, M., Terkaj, W., Mondellini, M., Colombo, G., *2022*. **Design of serious games in engineering education: An application to the configuration and analysis of manufacturing systems**. CIRP Journal of Manufacturing Science and Technology 36, 172–184. https://doi.org/10.1016/j.cirpj.2021.11.006
* Mahmood, K., Otto, T., Kuts, V., Terkaj, W., Modoni, G., Urgo, M., Colombo, G., Haidegger, G., Kovacs, P., Stahre, J., *2021*. **Advancement in production engineering education through Virtual Learning Factory Toolkit concept**. Proceedings of the Estonian Academy of Sciences 70, 374–382. https://doi.org/10.3176/proc.2021.4.02
* Terkaj, W., Qi, Q., Urgo, M., Scott, P.J., Jiang, X., *2021*. **Multi-scale modelling of manufacturing systems using ontologies and delta-lenses**. CIRP Annals 70, 361–364. https://doi.org/10.1016/j.cirp.2021.04.047
* Sanfilippo, E.M., Terkaj, W., Borgo, S., *2021*. **Ontological modeling of manufacturing resources**. Applied Ontology 16, 87–109. https://doi.org/10.3233/AO-210242
* Urgo, M., Terkaj, W., *2020*. **Formal modelling of release control policies as a plug-in for performance evaluation of manufacturing systems**. CIRP Annals 69, 377–380. https://doi.org/10.1016/j.cirp.2020.04.007
* Terkaj, W., Gaboardi, P., Trevisan, C., Tolio, T., Urgo, M., *2019*. **A digital factory platform for the design of roll shop plants**. CIRP Journal of Manufacturing Science and Technology 26, 88–93. https://doi.org/10.1016/j.cirpj.2019.04.007
* Terkaj, W., Tolio, T., Urgo, M., *2015*. **A virtual factory approach for in situ simulation to support production and maintenance planning**. CIRP Annals 64, 451–454. https://doi.org/10.1016/j.cirp.2015.04.121
* Kádár, B., Terkaj, W., Sacco, M., *2013*. **Semantic Virtual Factory supporting interoperable modelling and evaluation of production systems**. CIRP Annals 62, 443–446. https://doi.org/10.1016/j.cirp.2013.03.045