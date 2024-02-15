# 🧭 Dependency Map Project 
This project aims to create a visual map of dependencies between concepts. The map will help users navigate relationships and plan their learning.

## 🤔 What it does 
The dependency map gathers data on prerequisites between topics. It analyzes this data to create a network graph showing which concepts depend on others. This provides a "roadmap" to guide learning in an optimal order. 🧭

For example, the map may show that understanding addition is required before multiplication. Or that Newton's laws depend on kinematics concepts. By revealing these relationships, the map helps users efficiently build knowledge. 🧠

## How it works

Dependency data is collected from various sources like course materials. Each concept is represented as a node, while prerequisites become directed edges between nodes. 👥

The nodes and edges are then analyzed using network science algorithms. This includes partitioning them into layers, finding clusters, and calculating metrics like average path length. 🧮

Finally, the graph is visualized using force-directed layouts. This places strongly related topics closer together for easier browsing of the "map". Nodes can also be filtered and searched interactively. 🗺️

## 📚 Datasets

We analyzed two datasets:

1. Khan Academy Math Concepts - Extracted learning objectives and prerequisite relationships from Khan Academy math videos 🎥. Around 400 topics were used. 

2. Debian Software Dependencies - Contains packages and dependency relationships for Debian GNU/Linux distribution 🐧. Includes 27,623 packages and 48,138 dependencies. 

## 🧪 Methodology

The following steps were taken:

1. Extracted nodes (concepts, packages) and edges (prerequisites, dependencies) to build knowledge graphs 🧮

2. Performed graph layering to determine prerequisite "layers" 🧑‍🏫

3. Analyzed properties like degree distribution, diameter, density using NetworkX 🔬

4. Visualized graphs using ForceAtlas2 algorithm in Gephi 🌐

5. Discussed results and insights gained about network structure and learning pathways 💡

## 🛠 Tools Used

- Gephi for network graph generation and analysis🔧
- Custom Python scripts for preprocessing and analysis

## 📊 Results

Some key results:

- Scale-free structure with power law degree distribution observed
- Small world phenomenon seen with small diameters (Khan Academy = 8, Debian = 6)  
- Khan Academy graph is less dense(0.997) than Debian(0.999) due to smaller size
- Clustering reveals communities of semantically similar ideas.
- Layering revealed "levels" of prerequisites and dependency chains.

## 📖 References

The data sources and research papers referenced in the project are cited in the REFERENCES.md file.

👨‍💻 Developers

This project was developed by: Atthaluri Shashank

## 👨‍💻 Future Work

Potential extensions include:

- Larger and more diverse datasets 
- Dynamic graph analysis over time
- Community detection for related concepts/packages
- Recommendation systems based on graph structure

Let me know if any part of the analysis needs more explanation! Open to all suggestions to improve.

📚 Acknowledgements 📚
Thanks to all the past contributors and users who helped improve this project over the years! Special thanks to the Debian developers for the package dependency data. 
A Special thanks to Prof. G. Nagarjuna HBCSE Mumbai, India. who supervised me through out the project and taught me many life lessons which are still implemented by me everyday. 
