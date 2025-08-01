# 🧪 Delaney Solubility Dataset

The **Delaney Solubility Dataset** contains molecular data used to predict aqueous solubility (logS) of compounds. Understanding solubility is critical in drug discovery, as it helps determine whether a molecule will dissolve effectively in water or a given solvent — a key property for drug absorption and bioavailability.

## 📋 Dataset Structure

Each sample in the dataset represents a molecule, described by a set of calculated features:

| Feature               | Description                                                   |
|-----------------------|---------------------------------------------------------------|
| `MolLogP`             | Logarithm of the compound’s octanol-water partition coefficient (hydrophobicity) |
| `MolWt`               | Molecular weight                                              |
| `NumRotatableBonds`   | Number of rotatable chemical bonds (indicator of molecular flexibility) |
| `AromaticProportion`  | Proportion of aromatic atoms relative to total heavy atoms    |
| `logS`                | Target variable — log of aqueous solubility (mol/L)          |

```math
logS = f(MolLogP, MolWt, NumRotatableBonds, AromaticProportion)
```

## 📈 Why It Matters

Solubility directly affects:

- **Absorption**: Poor solubility limits a drug's effectiveness
- **Distribution**: Solubility influences how a drug spreads through the body
- **Formulation**: Helps in deciding excipients and dosage forms

By training a machine learning model on this dataset, we can build predictive tools to assess whether a molecule is likely to be a viable drug candidate based on its solubility.

## 🔗 Source

Originally published by **John Delaney**, this dataset has been widely used in computational chemistry and machine learning literature. A common version is available through the [DeepChem](https://deepchem.io/) project.

---
