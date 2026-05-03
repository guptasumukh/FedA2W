# FedA2W: Adaptive Aggregation with Weighted Loss Proximity for Non-IID Federated Learning

This repository serves as the **supplementary material** for the
research paper:

> "FedA2W: Adaptive Aggregation with Weighted Loss Proximity for
> Non-IID Federated Learning"

------------------------------------------------------------------------

## Repository Structure

. ├── datasets/ \# Dataset files used in the study 
. ├── results/ \# Best-performing client results on its testing split (CSV format)

------------------------------------------------------------------------

## Datasets

The repository includes multiple datasets spanning **vision, textual,
and tabular domains**:

### Vision Datasets

-   CIFAR-10
-   CIFAR-100

### Textual Dataset

-   Huffington Post Dataset
-   Symptom-Disease Dataset

### Tabular Datasets

-   NSL-KDD

All datasets used in the experiments are available in the `./datasets`
directory. The "train" file for CIFAR-100 has been split into 2 parts
"train_part1" and "train_part2"

------------------------------------------------------------------------

## Experimental Setup

-   The experiments simulate **real-world hetereogeneous and non-IID data distributions**
    using:
    -   Dirichlet's Distribution
    -   Label Skew
-   Each client receives:
    -   A **different number of samples**
    -   A **non-uniform class distribution**
-   The number of clients and test split details are provided in the
    research manuscript.

------------------------------------------------------------------------

## Results

The `./results` directory contains:

-   CSV files for the **best-performing client** on its local testing split
-   Each file includes:
    -   true labels
    -   predicted labels

- results_summary file that summarizes the correct/total labels and accuracy values (%)

### Note on Image Identifiers

For CIFAR datasets, no inherent IDs exist so identifiers are generated
programmatically during evaluation

They use binary batches which are just arrays of images by default

------------------------------------------------------------------------

## Notes

-   Results correspond to **best-performing client**
-   Dirichlet splitting introduces heterogeneity across clients

------------------------------------------------------------------------
