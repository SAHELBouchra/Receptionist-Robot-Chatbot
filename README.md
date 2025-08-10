# Receptionist-Robot-Chatbot

This repository contains the chatbot implementations designed to serve as the conversational language interface between a receptionist robot and humans. The chatbot enables natural and context-aware interaction, allowing the robot to understand and respond to user queries effectively.

## Project Overview

The chatbot is implemented in two versions:

- **Online Chatbot**: Utilizes the **Gemini Flash 1.5** language model via cloud API for generating responses.
- **Offline Chatbot**: Runs locally using the **Zephyr 7B Beta** model, allowing the chatbot to operate without an internet connection, optimized for edge devices.

Both versions employ a **Retrieval-Augmented Generation (RAG)** approach by retrieving relevant information from a knowledge base before generating answers, improving response accuracy and relevance.

## Features

- Retrieval-augmented generation for enhanced contextual understanding
- Two modes supporting both cloud-based and fully offline operation
- Designed for integration with receptionist robots for human-robot interaction
- Offline model optimized for running on resource-constrained hardware

## Getting Started

### Prerequisites

- Python 3.8+
- Dependencies listed in each chatbot folder’s `requirements.txt`
- For offline chatbot: Setup for Zephyr 7B Beta model weights and necessary libraries
- For online chatbot: Access and API credentials for Gemini Flash 1.5 cloud model

### Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/receptionist-robot-chatbot.git
cd receptionist-robot-chatbot
```
2. Choose the chatbot version you want to run (online_chatbot or offline_chatbot).

3. Install dependencies:
```bash
pip install -r requirements.txt
```
4. Prepare the knowledge base index if required (the .txt file).

5. Run the chatbot

## Usage
1. Runs as a terminal-based chatbot interface.

2. Retrieves relevant knowledge from the .txt knowledge base before generating responses.

3. Online chatbot requires valid API credentials and internet connection.

4. Offline chatbot runs locally with Zephyr 7B Beta model for inference without network.

## Notes
- Offline chatbot is suitable for edge deployment on devices with limited connectivity.
- Online chatbot leverages the Gemini Flash 1.5 model for up-to-date and high-quality responses.
- You can update the knowledge base text file and re-index to keep information current.
