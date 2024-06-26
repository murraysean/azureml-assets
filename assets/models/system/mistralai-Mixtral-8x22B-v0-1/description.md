The Mixtral-8x22B Large Language Model (LLM) is a pretrained generative Sparse Mixture of Experts.

Mixtral-8x22B-v0.1 is a pretrained base model and therefore does not have any moderation mechanisms.

# Evaluation Results 
[Open LLM Leaderboard Evaluation Results](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

Detailed results can be found [here](https://huggingface.co/datasets/open-llm-leaderboard/details_mistral-community__Mixtral-8x22B-v0.1)

|             Metric              |Value|
|---------------------------------|----:|
|Avg.                             |74.46|
|AI2 Reasoning Challenge (25-Shot)|70.48|
|HellaSwag (10-Shot)              |88.73|
|MMLU (5-Shot)                    |77.81|
|TruthfulQA (0-shot)              |51.08|
|Winogrande (5-shot)              |84.53|
|GSM8k (5-shot)                   |74.15|



# Inference samples

Inference type|Python sample (Notebook)|CLI with YAML
|--|--|--|
Real time|<a href="https://aka.ms/azureml-infer-online-sdk-text-generation-dolly" target="_blank">text-generation-online-endpoint.ipynb</a>|<a href="https://aka.ms/azureml-infer-online-cli-text-generation-dolly" target="_blank">text-generation-online-endpoint.sh</a>
Batch |<a href="https://aka.ms/azureml-infer-batch-sdk-text-generation" target="_blank">text-generation-batch-endpoint.ipynb</a>| coming soon

# Sample inputs and outputs

### Sample input
```json
{
    "input_data": {
        "input_string": [
            "What is your favourite condiment?",
            "Do you have mayonnaise recipes?"
        ],
        "parameters": {
            "max_new_tokens": 100,
            "do_sample": true,
            "return_full_text": false
        }
    }
}
```

### Sample output
```json
[
  {
    "0": "\n\nDoes Hellmann's Mayonnaise Mallows really exist?\n\nThis Punctuation Day Sign Maker was a playful way to celebrate Punctuation Day and to attempt to get more people involved in enjoyable punctuation practice that was creative. In this activity, learners were presented with a list of over 20 common punctuation or word processing symbols. They chose their favourite and then created a punctuation sign around it.\n\n## Preparation for this Pun",
    "1": " I would imagine that the ingredients consist, at least in large part, of oil and creamy things. Then there are eggs to hold it all together, salt and pepper for taste, and perhaps other flavourings depending on the tradition of any mayonnaise makers who attract your custom. A suitable theory of mayonnaise should surely tell us the function and contribution of these ingredients in a good mayonnaise.\n\nThe distinction between theories and recipes has been a theme in economics and in"
  }
]

```
