---
layout: project
type: project
image: img/raw.png
date: Summer 2025
published: False
labels:
  - LLM's
  - RAG
  - Agentic Pipeline
  - Bioinformatics
  - Research
---

## The Goal

During this summer internship my goal was to contribute research towards the potential and limitations of local LLM's using RAG and agents. Then use those findings to help a client in a bioinformatics projects where the client wanted the local LLM to be able to gather and organize data sets of different viruses then use that data to feed it into alphafold to try and find hotspots on the viruses data strands. Finally we were to take all of our teams research into a hackathon.

## What I Did

I successfully made a program using streamlit for the display and llama 3.2 for the LLM. My final program was able to take in a query from the user like: "Give me all the metadata for the mayaro virus," and then would use a RAG to go to two websites I specified: https://www.ncbi.nlm.nih.gov/ and https://www.iedb.org/
From those websites it would search for key words in the user inquiry and download any relevant as pdb files. Then I would use an agent with a hugging face model to chunk the information and gather all the information pertinent to what I needed. I would use a few more agents to do the same thing and then feed it to llama 3.2 for the LLM to find the commonality between the agents findings and feed those back to the RAG. I would then, using pandas, have that RAG output a neatly structured table for the client containing informations like: virus origin, a snippet of the viruses protein sequence, virus name, any sub viruses, etc.
The program also had a scoring based off of the confidence of the information output. If the confidence score was above a certain threshold, 90%, then I could give that information into alphafold and have alphafold make a 3d model of what the protein looks like which the client would take a look for "hotspots" on epitopes in the protein.

## Here is a link to the github page for source code

Source: <a href="https://uh-marketplace.github.io/"><i class="large github icon "></i>UH Marketplace</a>
