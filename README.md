# AI Data Analyst Workflow (n8n + LLMs)

<img width="1076" height="275" alt="automated data analyst" src="https://github.com/user-attachments/assets/6c3bcc1c-8cff-465b-8ab1-3d3fea6f7399" />




<img width="996" height="425" alt="output" src="https://github.com/user-attachments/assets/062dcddd-d6a4-4b78-8066-1d7bf30e620a" />



This repository documents an **AI-powered Data Analyst workflow** built with **n8n**, **Large Language Models (Groq & Google Gemini)**, **Google Sheets**, and **QuickChart**.  
The workflow converts natural language questions into structured analysis, visualizations, and professional email reports — fully automated end to end.

---

## Overview

The workflow behaves like a conversational data analyst.  
A user submits a question such as:

> *“What is the trend of life expectancy over the years?”*

The system automatically:
1. Interprets the analytical intent
2. Retrieves relevant data from Google Sheets
3. Structures and cleans the data
4. Generates multiple visualizations
5. Writes a concise executive-ready summary
6. Sends the results via email

---

## High-Level Architecture

```text
Chat Trigger
   ↓
AI Agent (Groq + Memory + Google Sheets Tool)
   ↓
Data Cleaning & Structuring
   ↓
Narrative Report Generation (Gemini)
   ↓
Chart Generation (QuickChart)
   ↓
Email Delivery (Gmail)
