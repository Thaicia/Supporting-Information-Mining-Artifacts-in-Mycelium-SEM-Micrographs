# Supporting-Information-Mining-Artifacts-in-Mycelium-SEM-Micrographs
Supporting information to preprint Mining Artifacts in Mycelium SEM Micrographs, Thaicia Stona de Almeida: mycelium pore map dataset

Paper available at https://arxiv.org/abs/2103.07573 (arXiv link)

The micrograph studied was provided by Ecovative Design LLC, in the context of the collaboration with Dr. Prathima Nalam's research project, 'Mechanics and Morphology of Mycelium', and Dr. Olga Wodo's research project, 'Modeling Quantitative Structure-Permeation Relationships for the Develop-ment of Mycelium-based Biodegradable Filtration Membranes', School of Engineering and Applied Sciences, State University of New York at Buffalo.

Preprint: Mining Artifacts in Mycelium SEM Micrographs

Abstract: Mycelium is a promising biomaterial based on fungal mycelium, a highly porous, nanofibrous structure. Scanning electron micrographs are used to characterize its network, but the currently available tools for nanofibrous microstructures do not contemplate the particularities of biomaterials. The adoption of a software for artificial nanofibrous in mycelium characterization adds the uncertainty of imaging artifact formation to the analysis. The reported work combines supervised and unsupervised machine learning methods to automate the identification of artifacts in the mapped pores of mycelium microstructure.

Keywords: Machine learning; unsupervised learning; image processing; mycelium; microstructure informatics

---

Content of file Dataset_PoreMap_Mycelium.xlsx:

poreID:  A unique number identifier for each pore counted in the image analyzed (pore map generated from SEM micrograph)

Area: List of all of the black pixel clusters’ numbers of black pixels that are not in a pore that touches the side of the image

Perimeter: The number of pixels in the perimeter of each pore.

Major: The length of the primary axis of the best fitting ellipse for each pore (major axis of ellipse)

Minor: The length of the secondary axis of the best fitting ellipse for each pore (minor axis of ellipse)

Angle: The angle between the major axis of the pore and a line parallel to the x-axis of the image

Circularity: (4π × [Area]) / [Perimeter^2] where a value of 1.0 indicates a perfect circle. As the value approaches 0.0, it indicates an increasingly elongated shape. Values may not be valid for very small pores

AspectRatio:  The aspect ratio of the particle’s fitted ellipse, i.e., [Major Axis] / [Minor Axis]

Roundness:  (4 × [Pore Area]) / (π × [Major axis]2) or the inverse of Aspect Ratio

Solidity: [Pore Area] / [Convex area of Pore]

Pore.Class: Proposed supervised classification of pores. The class can be regular (accurate identification of a pore), or an 
artifact of the image processing, shade or overlap (of fibers)

Class.Detail: A more detailed classification for purposes of unsupervised classification experiment and future work (e.g.: shade can be a background shade or a fiber shade)


![PoreMap_Mycelium_Highlighted_Small_Artifacts](https://user-images.githubusercontent.com/58062750/135920627-aae555e1-bdc5-4fd5-b475-e347d09846ba.png)

![OriginalOverlap_Highlighted](https://user-images.githubusercontent.com/58062750/135936989-540e3cc6-848a-44c5-91d4-3de4de077e1a.png)


