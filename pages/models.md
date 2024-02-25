# Models & update for models from OpenAI

Updated from [page OpenAI Models](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo)

As you can imagine, the models are continuously updated. Here is a summary of the models available at the time of writing this notebook (February 2024)

there are difference between text model (AKA GPT) and the model for image and voice recognition ( speech to text STS or text to speech TTS)


| Model | Description | Context Window | Training Data |
|-------|-------------|----------------|---------------|
| gpt-4-0125-preview | New GPT-4 Turbo: The latest GPT-4 model intended to reduce cases of “laziness” where the model doesn’t complete a task. Returns a maximum of 4,096 output tokens. | 128,000 tokens | Up to Dec 2023 |
| gpt-4-turbo-preview | Currently points to gpt-4-0125-preview. | 128,000 tokens | Up to Dec 2023 |
| gpt-4-1106-preview | GPT-4 Turbo model featuring improved instruction following, JSON mode, reproducible outputs, parallel function calling, and more. Returns a maximum of 4,096 output tokens. This is a preview model. | 128,000 tokens | Up to Apr 2023 |
| gpt-4-vision-preview | GPT-4 with the ability to understand images, in addition to all other GPT-4 Turbo capabilities. Currently points to gpt-4-1106-vision-preview. | 128,000 tokens | Up to Apr 2023 |
| gpt-4-1106-vision-preview | GPT-4 with the ability to understand images, in addition to all other GPT-4 Turbo capabilities. Returns a maximum of 4,096 output tokens. This is a preview model version. | 128,000 tokens | Up to Apr 2023 |
| gpt-4 | Currently points to gpt-4-0613. See continuous model upgrades. | 8,192 tokens | Up to Sep 2021 |
| gpt-4-0613 | Snapshot of gpt-4 from June 13th 2023 with improved function calling support. | 8,192 tokens | Up to Sep 2021 |
| gpt-4-32k | Currently points to gpt-4-32k-0613. See continuous model upgrades. This model was never rolled out widely in favor of GPT-4 Turbo. | 32,768 tokens | Up to Sep 2021 |
| gpt-4-32k-0613 | Snapshot of gpt-4-32k from June 13th 2023 with improved function calling support. This model was never rolled out widely in favor of GPT-4 Turbo. | 32,768 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-0125 | New Updated GPT 3.5 Turbo: The latest GPT-3.5 Turbo model with higher accuracy at responding in requested formats and a fix for a bug which caused a text encoding issue for non-English language function calls. Returns a maximum of 4,096 output tokens. | 16,385 tokens | Up to Sep 2021 |
| gpt-3.5-turbo | Currently points to gpt-3.5-turbo-0613. The gpt-3.5-turbo model alias will be automatically upgraded from gpt-3.5-turbo-0613 to gpt-3.5-turbo-0125 on February 16th. | 4,096 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-1106 | GPT-3.5 Turbo model with improved instruction following, JSON mode, reproducible outputs, parallel function calling, and more. Returns a maximum of 4,096 output tokens. | 16,385 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-instruct | Similar capabilities as GPT-3 era models. Compatible with legacy Completions endpoint and not Chat Completions. | 4,096 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-16k | Legacy: Currently points to gpt-3.5-turbo-16k-0613. | 16,385 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-0613 | Legacy: Snapshot of gpt-3.5-turbo from June 13th 2023. Will be deprecated on June 13, 2024. | 4,096 tokens | Up to Sep 2021 |
| gpt-3.5-turbo-16k-0613 | Legacy: Snapshot of gpt-3.5-16k-turbo from June 13th 2023. Will be deprecated on June 13, 2024. | 16,385 tokens | Up to Sep 2021 |