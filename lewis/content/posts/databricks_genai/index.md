+++
title = '2024 Databricks Generative AI World Cup'
date = 2025-03-28T00:00:00+00:00
+++

As part of the Renewable Energy Systems Ltd Data Science team, I competed in the [2024 Databricks Generative AI World Cup](https://hackathon.stackup.dev/web/events/generative-ai-world-cup-2024-so-you-think-you-can-hack) and placed 3rd inthe EMEA region.

The goal of this competition was to build an Generative AI solution using Databricks.

## Our Problem
We have lots of valuable textual data from engineers which detail past issues and resolutions. However, these are hard to search through and takes a lot of time to reading all relevant issues. 

What if we could search for semantically similar issues and use these to suggest a resolution for a new issue described by the engineer? 

## The Solution - Engineering Reccomendation Generator

We created a RAG system that uses vector search to show users similar engineering issues that have occurred in the past and uses these as context to suggest how to solve a new issue.

A streamlit UI is used to interact with the search engine.

![architecture](architecture_diag.png)

## Example Usage
![example](example_usage.png)

## References
Source code for submission is [here](https://github.com/res-ds/eng-rec-search).