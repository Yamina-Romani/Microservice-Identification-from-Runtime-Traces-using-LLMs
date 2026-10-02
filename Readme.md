# LLM-Assisted Microservice Identification from Monolithic Application Execution Traces

This repository contains the implementation and experimental materials for our approach to identifying
microservice candidates from runtime architectures.

The implementation uses runtime execution information and Large Language Models (LLMs) to identify potential
microservice boundaries.

This repository contains the notebook, input execution traces, and experimental results used for the LLM-assisted microservice identification approach.

## Requirements

- Google Colab
- Python 3
- The required Python packages are installed in the notebook.
- API keys for the LLMs used in the experiments.

## How to Execute the Notebook

1. Open the notebook located in the `Notebook/` folder.
2. Open the notebook in **Google Colab**.
3. Provide the required API keys in the corresponding cells.
4. Select the execution trace from the `Input/` folder.
5. Run the notebook cells sequentially.
6. The notebook processes the execution trace and generates the microservice decomposition results.

## Input

The `Input/` folder contains the execution traces used for the experiments.

```text
input/
├── jpetStore-traces
├── petClinic-traces
├── partsUnlimitedMRP-traces
└── 7ep-demo-traces
```

## Results

The `Generated Decompsitions/` folder contains the obtained microservice decompositions generated for the case studies.
```text
Generated Decompsitions/
├── JPetStore/
├── Spring-PetClinic/
├── PartsUnlimitedMRP/
└── 7ep-demo/
```
