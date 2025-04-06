# Optimization of Container Vessel Routing

This repository includes the data, pseudocode, and code used in the development of a methodology for optimizing the routing of container vessels. The approach is based on geographic clustering of ports and the subsequent optimization of both intra-cluster and inter-cluster routes.

## 📂 Repository Contents

### 📁 Data

- `instance_0` to `instance_12`: These 13 files correspond to each of the clusters generated during the geographic segmentation of ports.

- The following files contain global data for the complete set of ports:
  - `cap_port`: Port capacity in TEUs (Twenty-foot Equivalent Units).
  - `cap_vessel_port`: Vessel capacity per port.
  - `mov_teus_ports`: Number of containers to be moved from/to each port.
  - `vessel_info`: General information on vessels used in the study.

### 📄 Pseudocode

Two pseudocode files are included in plain text format:

- `pseudocodigo_clusterizacion.txt`: Pseudocode for the geographic clustering process using K-Means and the Haversine distance.
- `pseudocodigo_optimizacion.txt`: Pseudocode for the route optimization phase, considering port and vessel capacity constraints.

### 📓 Notebooks

- `clusterizacion.ipynb`: Clustering implementation using geographic K-Means and Haversine distance.
- `FVRP.ipynb`: Optimization of intra-cluster routes, addressing a capacitated Fleet Vehicle Routing Problem (FVRP).
- `medoides.ipynb`: Routing implementation between clusters using a medoid-based approach.

## 🎯 Project Objective

To develop a mathematical and algorithmic framework that enables the efficient routing of container vessels by:

- Incorporating Earth's curvature using Haversine distance
- Clustering ports based on geographic proximity and demand
- Optimizing vessel routes within and between clusters
- Considering vessel and port capacity constraints
- Minimizing logistical and environmental costs

## 🧪 Research Use

The results obtained were organized into instances to validate the methodology and to promote further research. Each instance includes port coordinates (latitude, longitude) and the number of TEUs to be moved. Detailed information for each instance is available in the uploaded files.

This repository can be used to:

- Validate maritime routing models
- Simulate container flow and fleet allocation
- Benchmark clustering and optimization approaches
- Support research on sustainable and intelligent maritime logistics

## 🤝 Contact

For more information or potential collaboration, feel free to contact:

- Author: Paola Alzate
- Email: paola.alzate4991@ucaldas.edu.co
- Institution / Research Group: Universidad de Caldas / Inteligencia Artificial

---

> 📌 **Note**: This repository is public and aims to support open data initiatives and reproducible research in the fields of operational research, transportation logistics, and maritime sustainability.
