Breaking Down Diffs: Can File-Wise Commit Message Generation Using LLMs Improve VCS Practices?

Commit messages play a crucial role in version control systems, providing essential context and explanations for changes made to the codebase. Despite their importance, many commit messages are poorly written or entirely missing, leading to challenges in code comprehension, bug tracking, and project maintenance. This paper addresses two significant issues in existing automated commit message generation approaches: the limitations of using datasets with short token lengths and the reliance on a single commit message for multiple file changes. To overcome these challenges, we generate commit messages for diffs with larger token lengths, using the latest LLMs, including GPT-4o, Llama 3.1 70B, Llama 3.1 8B, and Mistral Large. For evaluation, we conduct automatic assessments using metrics such as BLEU, ROUGE, METEOR, and CIDEr, as well as a human evaluation. Our findings indicate that GPT-4o and Llama 3.1 70B emerge as the best models for generating commit messages. Additionally, we propose a two-level approach that generates both an overall commit message and file-specific messages for each file change. To validate this approach, we surveyed developers to understand the problems they face with current commit messages and gather their feedback on our two-level approach. Our survey indicates that the two-level approach is effective and helps developers better understand complex and lengthy code diffs.

To run the code

You need to generate a API key for Hugging Face, Open AI, Mistral and Groq, given that the prerequisites to access models are available through the key.

Hugging Face: Mistral Tokenizer
OpenAI: GPT4o
Mistral: Mistral-Large
Groq: Llama3.1 70B and 8B

The code can be referred in SplitCommit.ipynb