# Quantum-Embedding-Kernels-Open-Project-QCG
Quantum Kernel SVM for Binary Classification
Overview
This project demonstrates the application of Quantum Embedding Kernels (QEKs) in a Support Vector Machine (SVM) framework for binary classification tasks. QEKs leverage quantum computing principles to map classical data into quantum states, enhancing the SVM's ability to discern complex patterns in the data.

Project Structure
1. Dataset Selection: We utilized the Iris dataset, focusing on two classes (Setosa and Versicolor), which were preprocessed and standardized for consistency.

2. Quantum Feature Mapping: Implemented using PennyLane, a quantum machine learning library, we defined a quantum circuit to encode classical data into quantum states. This circuit consists of RX and RY gates, which are variational parameters optimized to maximize the kernel-target alignment.

3. Quantum Kernel Calculation: The quantum kernel matrix is computed using the trained quantum circuit parameters. This matrix measures the similarity between each pair of data points in the feature space mapped to quantum states.

4. Optimization of Quantum Circuit Parameters: Using the COBYLA optimization method, we optimized the parameters of the quantum circuit to maximize the alignment between the quantum kernel matrix and the class labels (kernel-target alignment).

5. Noise Mitigation and Regularization: To improve the stability and generalization of the quantum kernel matrix, we applied noise mitigation techniques and regularization by adding a small value to its diagonal elements.

6. Training the SVM Classifier: We employed scikit-learn's SVM classifier with a precomputed kernel matrix derived from the quantum feature mapping. This SVM learns to classify new data points based on the optimized quantum kernel matrix.

7. Evaluation: The performance of the SVM classifier was evaluated on a hold-out test set. We computed classification accuracy to measure the effectiveness of our approach in distinguishing between Setosa and Versicolor classes.

Results
1. Quantum Kernel Matrix: Successfully computed and optimized using PennyLane's quantum circuit simulation.

2. Optimized Parameters: Identified optimal parameters for the quantum circuit that maximize kernel-target alignment.

3. SVM Classification Accuracy: Achieved a high classification accuracy of approximately 100% on the test set, showcasing the effectiveness of QEKs in enhancing SVM performance for binary classification tasks.

Conclusion
This project demonstrates the synergy between quantum computing and classical machine learning techniques, particularly in enhancing SVM classifiers using Quantum Embedding Kernels. The use of PennyLane for quantum simulation and scikit-learn for classical machine learning integration provides a robust framework for exploring quantum-enhanced algorithms in real-world applications.

