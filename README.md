# Medical Causal Reasoning in Large Language Models

This repository contains experimental code for evaluating domain-adapted ReAct prompting frameworks for medical causal reasoning tasks.

## 🎯 Overview

This study compares the effectiveness of different prompting strategies for medical causal reasoning:
* **Chain-of-Thought (CoT)** prompting
* **ReAct-Medical** domain-adapted framework
* **ReAct-Basic** generic reasoning framework
* **Zero-Shot** baseline approach

## 📁 Repository Structure

```
├── medical_causal_reasoning_experiment.ipynb           # Main experimental notebook
├── medical_causal_reasoning_experiment_output_20250608_070919.json  # Experiment results and outputs
├── README.md                                          # This file
```

## 🚀 Quick Start

### Prerequisites
* Python 3.7+
* OpenAI API key
* Jupyter Notebook or Google Colab

### Installation

1. **Clone the repository:**

```bash
git clone https://github.com/mahfuz-22/medical-causal-reasoning-llm.git
cd medical-causal-reasoning-llm
```

2. **Install dependencies:**

```bash
pip install openai pandas matplotlib numpy seaborn jupyter
```

3. **Set up OpenAI API key:**
   * Create a `.env` file in the root directory
   * Add your API key: `OPENAI_API_KEY=your_api_key_here`
   * Or set it directly in the notebook

### Running the Experiment

1. Open `medical_causal_reasoning_experiment.ipynb`
2. Run cells sequentially
3. Results will be displayed inline with visualizations
4. Complete results are saved in `medical_causal_reasoning_experiment_output_20250608_070919.json`

## 📊 Key Results

| Method | Accuracy | Performance Notes |
|--------|----------|-------------------|
| Chain-of-Thought | 91.7% | Best overall performance |
| ReAct-Medical | 66.7% | Domain-adapted, 60% improvement over baseline |
| ReAct-Basic | 41.7% | No improvement over baseline |
| Zero-Shot | 41.7% | Baseline comparison |

## 📄 Output Files

* `medical_causal_reasoning_experiment_output_20250608_070919.json`: Contains complete experimental results including:
   * Individual test case responses
   * Accuracy metrics for each prompting method
   * Detailed performance analysis
   * Timestamp: June 8, 2025, 07:09:19

## 🔧 Technical Details

* **Dataset**: 12 medical causal reasoning scenarios (literature-validated)
* **Model**: GPT-3.5-turbo
* **Evaluation**: Binary classification accuracy on causal inference tasks
* **Prompting Frameworks**: Chain-of-Thought, ReAct-Medical, ReAct-Basic, Zero-Shot
* **Total API Calls**: 48 (12 scenarios × 4 strategies)
* **Experiment Date**: June 8, 2025

## 🧪 Experimental Design

The experiment evaluates LLM performance on medical causal reasoning tasks including:
- Mediation scenarios (vaccination → antibodies → infection prevention)
- Confounding by indication (cholesterol medication ↔ heart attacks)
- Spurious correlations (ice cream sales ↔ drowning deaths)

Each scenario is tested across all four prompting strategies with consistent evaluation criteria.

## 📝 Citation

If you use this code in your research, please cite:

```bibtex
@misc{medical_causal_reasoning_2025,
  title={Evaluating Domain-Adapted ReAct Frameworks for Causal Reasoning in Large Language Models: A Medical Decision-Making Study},
  author={Mahfuz Rahman},
  year={2025},
  url={https://github.com/mahfuz-22/medical-causal-reasoning-llm}
}
```

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions about this research, please open an issue in this repository.

---

**Note**: This repository contains the complete experimental code and results referenced in our research paper "Evaluating Domain-Adapted ReAct Frameworks for Causal Reasoning in Large Language Models: A Medical Decision-Making Study". The JSON output file contains detailed results from the experiment conducted on June 8, 2025.
