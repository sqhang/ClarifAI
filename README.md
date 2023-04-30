# ClarifAI: Enhancing Audio-Based Question Answering with Whisper and GPT

This repository contains source files for Comp 646 final project, ClarifAI.
The goal of this project is to evaluate the performance of GPT-3.5 and GPT-4 on the SQuAD1.1 dataset and compare GPT-3.5 with state-of-the-art models like RoBERTa and DistilBERT on SQuAD and SpokenSQuAD datasets using audios of varying quality.
## Repository Contents

1. "audio_transcription.ipynb": This Jupyter Notebook contains code for speech-to-text conversion using the Whisper ASR model, generating datasets with audios of different quality levels, and creating audios with classroom noises. It also includes code for evaluating WER scores on these audios.

2. "GPT4 vs GPT3.5 Testing.ipynb": This Jupyter Notebook contains code for obtaining answers to the SQuAD1.1 dataset using GPT3.5 or GPT4 and generating JSON files with the answers.

3. "GPT3.5 Testing with audio transcripts.ipynb": This Jupyter Notebook achieves a similar goal as the previous one but uses audio transcripts from SpokenSQuAD of different quality levels as the "Context." It generates answers using GPT3.5 or GPT4 and creates JSON files with the answers.

4. "non_GPT_QA_models.ipynb": This Jupyter Notebook contains code for generating answers using RoBERTa and DistilBERT models with three types of contexts. It achieves the same goal as the previous notebooks but for these non-GPT models.

5. "Evaluation_scripts_for_all_jsons.ipynb": This Jupyter Notebook contains the compute_scores() function, which evaluates all the answers using the official SQuAD1.1 evaluation script. The function takes a JSON file and the SQuAD1.1 dev dataset as input and computes the evaluation scores (Exact Match and F1).


