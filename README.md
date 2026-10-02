# LLM-Assisted Microservice Identification from Execution Traces

This repository contains the implementation and experimental artifacts
for identifying microservice boundaries from monolithic application
execution traces using Large Language Models (LLMs).

The approach uses runtime behavioral information to construct three
complementary representations:

1. HTTP Route × Class interactions
2. Class co-occurrence
3. Class × Table/Operation interactions

These representations are provided to LLMs to generate candidate microservice decompositions. The same runtime evidence is also processed
using classical clustering algorithms for comparison.

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
├── 7ep-demo-traces.log
├── jpetstore-traces.log
├── partsUnlimitedMRP-traces.log
└── petclinic-traces.log
```
## Results
The Generated Decoposition/ folder contains the obtained microservice decompositions generated for the case studies.

```text
 Generated Decoposition/
├── 7ep-demo/
├── JPetStore/
├── PartsUnlimitedMRP/
└── Spring-PetClinic/
```
