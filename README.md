# Bangla Article Stance Detection Benchmark Dataset

A comprehensive benchmark dataset for stance detection in Bengali (Bangla) news articles, featuring human-annotated labels and classifications from multiple state-of-the-art Large Language Models (LLMs).

**Paper**: [Read Between the Lines: A Benchmark for Uncovering Political Bias in Bangla News Articles](https://arxiv.org/abs/2510.03898) (Accepted to BLP at AACL 2025)


## Dataset Structure

### Raw Data

The `raw_data/` directory contains the original dataset:

- **File**: `data.csv`
- **Format**: CSV
- **Columns**:
  - `ID`: Unique identifier for each article
  - `Event`: The event or topic the article discusses
  - `News Headline`: The headline of the news article
  - `News Body`: The full text content of the article
  - `Source Link`: URL to the original article
  - `Date`: Publication date
  - `News Corpora Name`: Source publication name (e.g., BBC Bangla, The Daily Star, Prothom Alo, etc.)
  - `final_label`: Human-annotated stance label

### Stance Labels

The dataset uses the following stance labels:

- **Govt critique**: Articles that are critical of the government
- **Govt leaning**: Articles that are supportive or favorable toward the government
- **Neutral**: Articles that maintain a neutral stance

### LLM Classifications

The `classified_by_llms/` directory contains stance classifications from various LLM models. Each file follows the naming convention: `{model-name}.csv`

**Included Models**:

- **Anthropic**: Claude Sonnet 4
- **DeepSeek**: DeepSeek-R1, DeepSeek-V3.1-Terminus
- **Google**: Gemini 2.5 Pro
- **Meta**: Llama 3.1 8B Instruct, Llama 3.3 70B Instruct
- **OpenAI**: GPT-4.1 Mini, GPT-5 Mini, GPT-OSS 20B, GPT-OSS 120B
- **Qwen**: Multiple variants (0.5B, 3B, 4B, 8B, 14B, 30B, 32B, 235B) including Instruct and Thinking variants
- **x-ai**: Grok-4 Fast
- **z-ai**: GLM-4.5
- **TigerLLM**: TigerLLM-9B-it

**Classification File Format**:
- `id`: Article identifier
- `article`: Full article text
- `headline`: Article headline
- `label`: Predicted stance label
- `reason`: Model's reasoning for the classification


## Use Cases

This dataset can be used for:

1. **Stance Detection Research**: Training and evaluating stance detection models for Bengali text
2. **LLM Benchmarking**: Comparing the performance of different LLM models on stance detection tasks
3. **Media Bias Analysis**: Analyzing media coverage and bias in Bengali news articles
4. **NLP Model Development**: Developing and fine-tuning natural language processing models for Bengali
5. **Cross-lingual Studies**: Comparing stance detection approaches across different languages

# Data Use Agreement

This dataset is released for **scholarly, academic, and research purposes only**.

By accessing or using this dataset, you agree to the following terms:

## Permitted Use
- You may use this dataset for **non-commercial academic research**, 
  publications, teaching, and student projects.

## Prohibited Use
- **Commercial use is strictly prohibited.**
- Use in commercial products, services, or for monetization of any kind
  requires explicit written permission from the dataset creator.
- Redistribution of the dataset without permission is not allowed.

## Citation Requirement
If you use this dataset in any publication, project, or presentation, you must
include the following citation:


## Citation

If you use this dataset in your research, please cite:

```bibtex
@article{lia2025read,
  title={Read Between the Lines: A Benchmark for Uncovering Political Bias in Bangla News Articles},
  author={Lia, Nusrat Jahan and Dipta, Shubhashis Roy and Zehady, Abdullah Khan and Islam, Naymul and Chakraborty, Madhusodan and Wasif, Abdullah Al},
  journal={arXiv preprint arXiv:2510.03898},
  year={2025}
}
```

**Paper Website**: [https://nusrat-lia.github.io/BanglaBias/](https://nusrat-lia.github.io/BanglaBias/)


## Additional Notes
- All users must comply with ethical research practices.
- The dataset is provided "as is" without warranties.


## Acknowledgments

- All news sources that provided the original articles
- Contributors who annotated the dataset
- The LLM providers whose models were used for classification


