# Abstract

This report applies graph analytics methods to analyze the curriculum structures of MSc programs in Data Science, Statistics, and Data Analytics. The study aims to uncover relationships between courses, units, and subtopics, providing data-driven insights for curriculum optimization and cross-program integration. Using NetworkX, a graph is constructed representing courses, units, and subtopics as nodes at different hierarchical levels, with edges denoting various relationships. Cosine similarity, based on TF-IDF vectorization of subtopic descriptions, quantifies connections between subtopics both within and across programs. Multiple centrality measures identify influential nodes, while community detection algorithms uncover clusters of closely related topics.
The analysis reveals several key findings. Central courses and units critical for information flow across the curriculum are identified. Distinct topic communities are detected, revealing underlying program structures and potential specialization tracks. Significant cross-program similarities are discovered, highlighting opportunities for interdisciplinary integration. The study also identifies potential curriculum gaps and redundancies, and reveals optimal pathways for concept progression throughout the programs.
The analytical approach employs various techniques, including graph construction using NetworkX, similarity quantification using cosine similarity and TF-IDF, centrality analysis (degree, betweenness, eigenvector centrality), community detection (Louvain method, modularity optimization), and interactive visualizations using Plotly. This comprehensive methodology enables a multi-faceted examination of the curriculum structures.
The implications of this study are far-reaching. It provides a data-driven basis for refining course content and structure, and offers opportunities for developing interdisciplinary courses or modules. The findings create a framework for adaptive, personalized learning pathways and have the potential to align academic programs more closely with industry skill requirements.
Moreover, the approach establishes a foundation for ongoing curriculum assessment and improvement.

# Introduction

In the rapidly evolving landscape of data science and analytics, the interconnection of curriculum concepts across related disciplines like MSc Data Science, MSc Statistics, and MSc Data Analytics is crucial for fostering a comprehensive understanding of the field. This project aims to explore and analyze the relatedness and importance of these curriculum concepts using advanced graph analytics methods.
By constructing a network of concepts where nodes represent individual topics and edges denote their relationships, this study delves into the intricate web of connections that bind these disciplines together. The project further employs centrality measures to identify the most influential and pivotal nodes within the network, thereby highlighting key concepts that serve as the foundation for these programs.
In addition, community detection algorithms are utilized to uncover clusters of closely related concepts, offering insights into the natural grouping of topics within the curriculum. Sub-graphs are also visualized to provide a detailed examination of specific areas, enabling a deeper understanding of how certain concepts are interrelated.
This comprehensive analysis not only underscores the significance of interconnected concepts in the curriculum but also provides a rationale for the structure and content of these academic programs. The findings of this project are presented with a detailed interpretation, offering valuable insights for educators and curriculum designers in refining and optimizing educational content for future cohorts.
This project aims to explore these aspects by applying graph analytics methods to the curriculum structures of three Master's programs: MSc Data Science (MDS), MSc Statistics (MST), and MSc Data Analytics (MDA).

# Objectives

1.1NETWORK CREATION AND EDGE IDENTIFICATION<br>
o Did manual imputation to preprocess the data and then converted them to
dictionary and further to json files.<br>
o Use cosine similarity to identify and visualize connections between subtopics.
This involves calculating within-unit similarities, cross-unit similarities, and
cross-program similarities to establish the edges between nodes.<br>
2 CENTRALITY MEASURES<br>
o Apply centrality measures to identify important nodes within the graphs. This
includes evaluating which units or subunits hold significant positions in the
network, providing insights into their relevance and impact on the overall
curriculum structure.<br>
3 COMMUNITY DETECTION AND VISUALIZATION<br>
o Detect and visualize communities within the network graphs. Communities
represent groups of nodes with higher interconnectivity compared to nodes
outside their group.<br>
4 SUB-GRAPH VISUALIZATION<br>
o Create and visualize detailed sub-graphs to illustrate specific aspects of the
curriculum structure, such as the relationship between subunits within a unit or
between units of different programs. These visualizations will aid in a more
granular analysis of curriculum similarities and differences.

# Conclusion

The study successfully developed and implemented several major modules, beginning with data extraction and preprocessing from syllabus documents. This crucial first step laid the foundation for subsequent analyses. The graph creation and visualization module transformed the preprocessed data into a network structure, providing a visual representation of the curriculum's interconnectedness. The centrality analysis module applied various metrics to identify influential nodes within the network, highlighting courses and units critical for information flow and concept integration across the programs.
Community detection algorithms were employed to uncover clusters of related topics, revealing the underlying structure of the curriculum and potential areas for cross-program integration. The subgraph analysis module allowed for a more focused examination of specific relationships within the larger network, providing detailed insights into particular areas of the curriculum.
Through these analyses, the study successfully created a comprehensive graph representation of the curriculum structure, identifying influential nodes and communities. Centrality measures revealed key courses and units that serve as critical junctures for information flow within and between programs. The community detection algorithms uncovered clusters of related topics, shedding light on the natural groupings of concepts across the different programs. The various visualizations developed throughout the project provided intuitive and informative representations of the curriculum structure and relationships, making complex data more accessible to stakeholders.
Despite these successes, the study acknowledges certain limitations, primarily the reliance on text-based similarity for establishing connections between curriculum components. This approach, while effective, may not capture all pedagogical relationships or the nuanced connections between topics that exist in practice. Future enhancements to this project could address these limitations by incorporating additional data sources and analytical techniques.
Looking ahead, there are several promising avenues for expanding and refining this work. Incorporating student performance data could provide insights into the effectiveness of the current curriculum structure and highlight areas for improvement. Integrating industry feedback could ensure that the curriculum remains aligned with evolving market demands. Considering the temporal aspects of the curriculum could offer a more dynamic view of how concepts build upon each other throughout a student's academic journey.
