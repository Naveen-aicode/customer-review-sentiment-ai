# AI-Powered Customer Review Analysis with Gemini

An AI-powered customer feedback analysis project built using Google Cloud, BigQuery, Gemini, Vertex AI, and Python.

The project analyzes customer reviews from text and audio sources, classifies sentiment, summarizes customer feedback, extracts keywords, and generates actionable recommendations for improving customer experience.

---

## 🚀 Project Overview

Customer feedback can come from multiple channels such as social media, online reviews, and audio recordings.

This project demonstrates how Generative AI can be used to process both **text-based and audio-based customer feedback** and convert unstructured feedback into useful business insights.

The project uses:

- **Google BigQuery** for storing and querying customer review data
- **Gemini 2.5 Flash** for Generative AI analysis
- **BigQuery ML.GENERATE_TEXT** for text sentiment classification
- **Vertex AI** for audio analysis
- **Google Cloud Storage** for accessing customer review audio files
- **Python** for data processing and visualization

---

## 🎯 Objectives

The main objectives of this project are to:

1. Load customer review data into BigQuery.
2. Analyze customer reviews using Gemini.
3. Classify reviews as positive or negative.
4. Clean and standardize the generated sentiment results.
5. Summarize sentiment distribution.
6. Process audio customer reviews using Gemini.
7. Generate transcripts from audio.
8. Extract keywords and summarize customer feedback.
9. Generate customer-service responses.
10. Recommend actions that businesses can take to improve customer experience.

---

## 🏗️ Architecture

```text
                    Customer Feedback
                           |
              +------------+------------+
              |                         |
         Text Reviews              Audio Reviews
              |                         |
              v                         v
        Google Cloud               Google Cloud
         Storage /                 Storage Audio
         BigQuery                       |
              |                         |
              v                         v
        BigQuery ML              Vertex AI + Gemini
              |                   Gemini 2.5 Flash
              v                         |
       Gemini 2.5 Flash                 |
              |                         |
              v                         v
      Sentiment Analysis       Transcript + Summary
              |                + Keywords + Sentiment
              |                + Customer Response
              |                + Recommended Actions
              |                         |
              +------------+------------+
                           |
                           v
                   Customer Insights
