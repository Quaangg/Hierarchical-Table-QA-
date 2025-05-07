# **Hierarchical Table QA with TAPAS and TAPEX on the HiTab Dataset**

## **Project Overview**

This project investigates the performance of two pre-trained Table-to-Text QA models—**tapas-large-finetuned-wtq** and **tapex-large-finetuned-wtq**—on the **HiTab dataset**, which consists of hierarchical tables and multi-layered questions. To address the unique challenges posed by this dataset, **TAPEX** was further fine-tuned to enhance its ability to reason over complex tabular structures. The study highlights the limitations of existing models and explores new directions in hierarchical table-based question answering (QA).

## **Datasets**

1. **HiTab Dataset**:

   * **Source**: [HiTab Dataset](https://github.com/microsoft/HiTab)
   * **Description**: A dataset containing hierarchical tables with multi-layered questions. It presents significant challenges for existing baselines and provides new opportunities for research in processing hierarchical tabular data for QA tasks.
   * **Data Columns**: Structured tables with rows and columns containing both numerical and textual information.

2. **Pretrained Models**:

   * **TAPAS-large-finetuned-wtq** and **TAPEX-large-finetuned-wtq** are used as baseline models for comparison.

## **Input and Output Format**

### **Input**:

* **Tabular data**: Structured tables with multiple rows and columns, containing numerical and textual information.
* **Question**: A natural language query, either directly asking for a specific value or requiring reasoning across multiple sections of the table.

### **Output**:

* **Answer**: A concise and accurate response inferred from the table and question, which can be a specific value (numerical or textual) or a result derived from computations over the data.

## **Methodology**

1. **Data Preprocessing**:

   * The dataset was processed to convert tables into a structured format suitable for QA tasks. Preprocessing steps included normalizing tables and preparing question-answer pairs.
2. **Model Training**:

   * **TAPEX** and **TAPAS** models were fine-tuned on the HiTab dataset to optimize their performance on hierarchical table-based reasoning tasks.
3. **Evaluation**:

   * Models were evaluated using various QA metrics, including **accuracy** and **F1-score**, to determine their effectiveness at handling multi-layered questions over tabular data.

## **Key Contributions**

* **Empirical comparison** of **TAPAS** and **TAPEX** on hierarchical tabular QA tasks using the HiTab dataset.
* **Fine-tuning TAPEX** to improve performance on complex, multi-level tables.
* **Identification of model limitations** and exploration of new research directions for advancing hierarchical table understanding in QA systems.

## **Installation**

### Prerequisites:

Ensure that you have **Python 3.x** installed. Then, install the required libraries using pip:

```bash
pip install pandas numpy scikit-learn transformers
```

### **How to Use**

1. **Clone the Repository**:
   First, clone the repository to your local machine:

   ```bash
   git clone https://github.com/Quaangg/Hierarchical-Table-QA.git
   ```

2. **Download the HiTab Dataset**:

   * The **HiTab Dataset** can be downloaded from the official repository: [HiTab Dataset on GitHub](https://github.com/microsoft/HiTab).

3. **Run the Models**:
   Follow the instructions in the repository to train and fine-tune the **TAPEX** and **TAPAS** models on the HiTab dataset.

## **GitHub Repository**

* **Link to GitHub Repository**: [Hierarchical-Table-QA](https://github.com/Quaangg/Hierarchical-Table-QA)

## **Project Duration**

6 weeks

## **Conclusion**

This research demonstrates the challenges and opportunities in hierarchical table-based question answering. By fine-tuning **TAPEX**, we have shown improvements in processing multi-layered tables and answering complex queries. The results contribute valuable insights into the development of QA systems capable of handling hierarchical tabular data.
