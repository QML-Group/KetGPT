<img src="logo.png" alt="drawing" width="50"/> #KetGPT

## Dataset Augmentation of Quantum Circuits using Transformers

This repository hosts the accompanying software for the following research article and master thesis. 

#### Abstract (research article):

Quantum algorithms, represented as quantum circuits, can be used as benchmarks for assessing the performance of quantum systems. Existing datasets, widely utilized in the field, suffer from limitations in size and versatility, leading researchers to employ randomly generated circuits. Random circuits are, however, not representative benchmarks as they lack the inherent properties of real quantum algorithms for which the quantum systems are manufactured. This shortage of `useful' quantum benchmarks poses a challenge to advancing the development and comparison of quantum compilers and hardware. 

This research aims to enhance the existing quantum circuit datasets by generating what we refer to as `realistic-looking' circuits by employing the Transformer machine learning architecture. For this purpose, we introduce KetGPT, a tool that generates synthetic circuits in OpenQASM language, whose structure is based on quantum circuits derived from existing quantum algorithms and follows the typical patterns of human-written algorithm-based code (e.g., order of gates and qubits). Our three-fold verification process, involving manual inspection and Qiskit framework execution, transformer-based classification, and structural analysis, demonstrates the efficacy of KetGPT in producing large amounts of additional circuits that closely align with algorithm-based structures. Beyond benchmarking, we envision KetGPT contributing substantially to AI-driven quantum compilers and systems.

#### Abstract (masters thesis):

The goal of this thesis is expanding quantum algorithm datasets to enhance our capability to benchmark quantum systems and to open up possibilities for using machine learning techniques in quantum circuit mapping. Both of these areas are currently hindered by the lack of a wide range of useful quantum algorithms. To solve this problem, KetGPT is presented, a model that uses the revolutionary transformer machine learning architecture to generate synthetic, yet realistic looking, quantum circuits. By visual inspection, KetGPT generated circuits are easily distinguishable from random circuits, and show desirable qualities such as structure and human-like programming factors including applying gates in the order of ascending qubits. Consequently, they might be more suitable for certain tasks like benchmarking and training a reinforcement learning compiler. In an attempt to quantify the quality of circuits generated by KetGPT, a separate transformer classifier model was trained on the task of classifying the synthetic circuits generated by KetGPT as either real circuits, or as random circuits. However, although this classifier might capture realistic features of quantum circuits, the classifier has not been unambiguously proven to be reliable, and can therefore not be used as a standalone tool to determine the quality of KetGPT generated quantum circuits. Nevertheless, KetGPT and the transformer classifier are novel, promising approaches in an attempt to expand quantum algorithm datasets.

#### Software and Data availability:

The final version of the KetGPT software is available as a Notebook on Google Colaboratory. Please access it [here](https://colab.research.google.com/drive/1dbtJX6q8sED4yrb1I09KUuXWYH0AVN8r).

The data that was used for this work, comprising of the training dataset, and a KetGPT folder that contains: the pre-trained KetGPT model, the KetGPT tokenizer, the pre-trained classifier model, all KetGPT generated circuits and all random circuits, is available [here](https://www.kaggle.com/datasets/boranapak/ketgpt-data).

