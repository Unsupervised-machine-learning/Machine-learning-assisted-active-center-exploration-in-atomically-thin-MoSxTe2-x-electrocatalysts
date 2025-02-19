# Machine learning-assisted active center exploration in atomically thin MoSxTe2-x electrocatalysts for efficient hydrogen evolution
## Abstract
Modulating the local configurations has been widely considered an efficient strategy to promote the catalytic performance of 2D molybdenum disulfide (MoS2) for hydrogen evolution reaction (HER). Although transmission electron microscopy prevails as a central tool to visualize catalysts at atomic resolution, there still lacks a rapid and accurate approach to find out the active centers in the micrographs containing abundant structural information. Herein, we create a defective MoSxTe2-x alloy catalyst through low-temperature sulfurization of 1T′-MoTe2 (S-MoTe2), whose atomic structure is automatically explored using an unsupervised machine learning (ML) framework based on Zernike feature and uniform manifold approximation and projection (UMAP)-based dimension-reduced K-means clustering, enabling the discovery of a novel defect configuration referred antisite Te adatom (Teads-Mo). Density functional theory (DFT) calculations reveal a synergistic enhancement in both the hydrogen adsorption capability and electronic conductivity of these antisite defects, which is experimentally verified by the half-reduced overpotential and Tafel slope of S-MoTe2 alloy compared to its counterparts (tellurization of 2H-MoS2, denoted as Te-MoS2). This work provides an intelligent approach to facilitate active center exploration in micrographs and achieves a closed-loop verification for the ML-assisted defect discovery via theoretical calculations and electrochemical experiments, displaying how ML and researchers seamlessly cooperate in a scientific workflow for advanced catalyst development.
## Machine learning project tasks
The project is divided into two tasks: task1 is used to discover antisite Te adatoms, and task2 is used to quantitatively analyze Te-based configurations including both antisite Te adatoms and Te substitutions. The project is implemented in Python 3.8 and involves tasks such as atomic point detection, feature extraction, dimensionality reduction, clustering, visualization,and model assessment. The analysis and processing are done using Jupyter Notebooks.

## Installing Dependencies

Before using this project, ensure that Python 3.8 is installed and the required dependencies are in place:

1. Clone the repository:

   ```bash
   git clone <git repo>
   cd <repo path>
   ```

2. Create and activate a virtual environment (optional, but recommended):

   ```bash
   conda create -n atom python=3.8
   conda activate atom
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Task Workflow

This project performed using Jupyter Notebooks.

### Stage 1: Point Detection

Run `Stage1-Point-Detection.ipynb` for atomic point detection.

1. Open `Stage1-Point-Detection.ipynb` and run all the code cells.
2. This stage will output the coordinates or relevant information for the detected atomic points.

### Stage 2: Feature Extraction, Dimensionality Reduction, Clustering, and Visualization

After completing point detection, run `Stage2-ZP-UMAP-Kmeans.ipynb` for atomic feature extraction, dimensionality reduction, clustering, and visualization.

1. Open `Stage2-ZP-UMAP-Kmeans.ipynb` and run all the code cells.
2. In this stage, you will:
   - Extract atomic features;
   - Perform dimensionality reduction;
   - Use the K-means clustering algorithm for clustering;
   - Visualize the clustering results.
### Stage 3: Model Assessment

After completing the visualization of the clustering results, run `Stage3-Model-Assessment.ipynb` for model assessment.

1. Open `Stage3-Model-Assessment.ipynb` and run all the code cells.
2. This stage will output the classification metrics of structural motifs including accuracy, precision, recall and F1 score according to the corresponding ground truth.
## File Structure

```
your_project_directory/
│
├── requirements.txt                                                         # Dependencies file
├── task1-Discovery of antisite Te adatoms                                   # code and data for task1
├── task2-Quantitative analysis of Te-based configurations                   # code and data for task2
└── README.md                                                                # Project documentation
```

## License

This project is licensed under the [MIT License](LICENSE).
