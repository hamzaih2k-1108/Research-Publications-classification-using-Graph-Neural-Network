
# Research Publications Classification Using Graph Neural Networks  

This repository contains a project for classifying research publications based on their content and metadata using **Graph Neural Networks (GNNs)**. By leveraging graph-based representations of publication data, the project demonstrates how GNNs can effectively capture relationships and patterns for accurate classification.

## Table of Contents  
1. [Introduction](#introduction)  
2. [Dataset](#dataset)  
3. [Architecture](#architecture)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Results](#results)  
7. [Contributing](#contributing)  
8. [License](#license)  

---

## Introduction  

Graph Neural Networks have shown significant promise in various domains, especially where data can be represented as graphs. In this project:  
- **Nodes** represent research publications.  
- **Edges** capture relationships such as citations, shared authors, or shared keywords.  

The objective is to classify research papers into predefined categories using GNNs while exploring their capabilities in handling structured and unstructured data.

---

## Dataset  

The dataset consists of:  
1. **Node Features**: Attributes derived from the publication text (e.g., TF-IDF vectors, embeddings).  
2. **Edge Information**: Citation networks or co-authorship connections between publications.  
3. **Labels**: Ground-truth categories or topics of the publications.  

*Note*: Preprocessing steps for feature extraction and graph construction are included in the code.

---

## Architecture  

The project employs the following architecture:  
1. **Graph Construction**: Creating a graph representation from the dataset.  
2. **Graph Neural Network Model**: Implementation of a GNN using frameworks like PyTorch Geometric or DGL.  
    - GNN variants such as GCN, GAT, or GraphSAGE can be used.  
3. **Training and Evaluation**: Supervised learning with loss functions and metrics like accuracy or F1-score.  

---

## Installation  

### Prerequisites  
Ensure you have the following installed:  
- Python 3.8 or higher  
- PyTorch  
- PyTorch Geometric (or DGL)  
- Scikit-learn  
- Pandas  

### Installation Steps  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/hamzaih2k-1108/Research-Publications-classification-using-Graph-Neural-Network.git  
   cd Research-Publications-classification-using-Graph-Neural-Network  
   ```  
2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

---

## Usage  

### Preprocessing  
To preprocess the dataset and create the graph:  
```bash  
python preprocess.py  
```  

### Training the Model  
To train the GNN:  
```bash  
python train.py --model GCN --epochs 100  
```  

### Evaluation  
Evaluate the trained model on the test set:  
```bash  
python evaluate.py --model_path saved_model.pth  
```  

### Visualization  
Visualize the graph and results:  
```bash  
python visualize.py  
```  

---

## Results  

The GNN achieved the following performance:  
- **Accuracy**: XX%  
- **F1-Score**: XX%  
- **Precision**: XX%  
- **Recall**: XX%  

*Detailed results and analysis can be found in the `results/` folder.*  

---

## Contributing  

Contributions are welcome! If you find bugs, have suggestions, or want to add new features, please submit an issue or a pull request.  

---

## License  

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.  

---

## Acknowledgments  

This project is inspired by the growing importance of GNNs in scientific document classification and builds upon the tools provided by PyTorch Geometric and other open-source libraries.

