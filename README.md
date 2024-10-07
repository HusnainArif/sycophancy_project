# Jury-Based Multi-Faceted Sycophancy Detection in LLMs

## Overview

This project delves into the phenomenon of sycophancy in Large Language Models (LLMs), specifically focusing on the Gemma2 family of models. Sycophancy refers to the tendency of these models to align their responses with user opinions, even at the expense of objective truth. This research introduces a novel, granular approach to evaluating and measuring sycophantic behavior, alongside a jury-based methodology for multi-faceted detection and analysis.

YouTube video: [link](https://www.youtube.com/watch?v=oC49Yb55RH4&t=861s&ab_channel=HusnainArifWahla)

Project slides: [link](https://gamma.app/docs/Jury-Based-Multi-Faceted-Sycophancy-Detection-in-LLMs-y7dpskdpujr2gf5?mode=doc)

## What is Sycophancy?

Sycophancy in LLMs refers to the tendency of the model to align its responses with user views, even if the statements are factually incorrect. This can lead to models that prioritize user satisfaction over truthfulness, potentially reinforcing biases and contributing to echo chambers in society.

## General Observations

- **Model Size:** Larger models tend to be more sycophantic as they can better detect and adapt to user beliefs.
- **Reinforcement Learning with Human Feedback (RLHF):** RLHF usually amplifies sycophantic tendencies as models focus on user satisfaction.
- **Types of Sycophancy:** Two types; `Objective Sycophancy` (where a right answer exists) and `Subjective Sycophancy` (no definitive answer).

## Dataset

The dataset for this study was constructed using GPT-4o to generate questions across 10 political topics, with user opinions and arguments crafted for each question.

## Experiment Setup

The project involved testing three Gemma2 models (2B, 9B, and 27B) on political and opinion-based questions using various interventions:
1. **User Opinion**
2. **User Hobby**
3. **Strong Argument**
4. **Weak Argument**

### AI Jury Structure

The evaluation is conducted using a jury of three LLMs:
- GPT-4o
- Claude Sonnet-3.5
- Llama-3.1-405B

Each juror assesses the model's responses before and after interventions to determine if sycophantic behavior is present.

## Evaluation Process

1. **Scenario Setup:** Initial model response to a question is recorded.
2. **Intervention:** The model is confronted with conflicting user input.
3. **Response Analysis:** The jury analyzes the model's response shift.
4. **Verdict:** The decision is based on a majority vote among the jurors.

## Key Contributions

- **Granular Analysis:** Evaluation of how different interventions (user opinion, hobbies, strong/weak arguments) affect model behavior.
- **Multi-Interaction Analysis:** Comparison of model stances before and after interventions.
- **Reasoning Emphasis:** Focus on underlying reasoning behind model behavior changes.

## Experiment Results

- **User Opinions:** Generated the highest sycophancy scores.
- **Weak Arguments:** Models showed the least sycophantic behavior.
- **Model Size Analysis:** Larger models did not always show the highest sycophancy, with some variations based on the type of intervention.

## Contact

For more information, please feel free to reach out to me :)
