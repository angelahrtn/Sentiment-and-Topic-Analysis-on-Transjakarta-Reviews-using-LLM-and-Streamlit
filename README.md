# Transjakarta Insight Review: Sentiment & Topic Analysis
# Project Overview
This project was developed to analyze customer reviews about Transjakarta services collected from various social media platforms. The goal is to understand public sentiment (positive, neutral, negative) and uncover key discussion topics using a Large Language Model (LLM).

By combining sentiment analysis and topic modeling, the application provides actionable insights for Transjakarta staff to evaluate public perception, identify recurring issues, and improve service quality.

The model and visualizations are deployed through Streamlit, enabling an interactive and user-friendly web application where users can explore the analysis in real time.

# Case Description
Public feedback plays an important role in improving transportation services. However, the large volume of unstructured text data on social media makes manual analysis impractical.

This project addresses that challenge by:
- Collecting user-generated reviews about Transjakarta via web scraping.
- Using an LLM-based classification model to predict the sentiment of each review.
- Grouping the reviews into topics based on their sentiment category.
- Displaying the insights interactively using Streamlit, making it accessible to non-technical users such as Transjakarta staff.

The insights help identify what aspects of the service are most frequently praised or criticized — such as waiting time, payment system, bus availability, app usability, and station facilities.

# Objectives
- Perform Sentiment Analysis to classify reviews into Positive, Neutral, and Negative.
- Perform Topic Analysis to extract key issues or themes from each sentiment category.
- Utilize LLM-based models for high-quality text understanding and classification.
- Deploy the application using Streamlit to make insights easily accessible to decision-makers.
- Provide intuitive visualizations, including bar charts, word clouds, and review examples per sentiment.

# Project Steps and Features
1. Data Collection and Preprocessing
- Data was collected through scraping from multiple social media sources related to Transjakarta.
- The collected reviews were manually labeled by three annotators into sentiment categories before preprocessing.
- Text cleaning and preprocessing were performed (lowercasing, punctuation removal, stopword filtering, etc.).
- Each review was stored with metadata such as source, date, and word count.

2. Sentiment Prediction using LLM
- A pretrained Large Language Model (LLM) was used to predict sentiment categories:
- Negative, Neutral, and Positive.
- Model outputs were verified and cleaned to ensure consistent labeling.

3. Topic Analysis
- Within each sentiment class, the reviews were grouped into key topics using a combination of:
  - Semantic similarity,
  - LLM-based clustering,
  - Keyword extraction.
- Example topics include:
  - Layanan Transjakarta (Transjakarta Services)
  - Sistem Pembayaran: Tap In/Out
  - Waktu Tunggu (Waiting Time)
  - Ketersediaan Armada (Fleet Availability)

4. Visualization and User Interface
- Built using Streamlit for interactive exploration.
- Features include:
  - Sentiment distribution charts
  - Topic frequency bar charts
  - Word clouds per sentiment
  - Sample review table for qualitative understanding

5. Deployment
- The final application was deployed to Streamlit Cloud:
  👉 https://transjakarta-reviews-insight.streamlit.app/
- The app allows real-time exploration of sentiment and topic trends.
