# Ollama Chat API

## Overview

The Ollama Chat API is a Spring Boot application that allows users to interact with AI models for conversational purposes. It provides a REST API endpoint where users can send messages and receive responses from an AI model powered by Ollama.

## Project Structure

1. **`OllamaChatController`**:
   - Handles HTTP requests for chatting with the AI model.
   - Uses the Ollama AI model to process user messages and return responses.

2. **`OllamaChatService`**:
   - Configures and provides the `ChatClient` bean for interacting with the Ollama AI model.
   - Handles the communication with the Ollama API.

3. **`ApplicationProperties`**:
   - Provides configuration properties for `OllamaChatService`like using Mistral or Llama model

## Configuration

1. **Set up your environment**:
   - Ensure you have Java 17 and Gradle installed.

2. **Configure the application properties**:
   - Update `src/main/resources/application.properties` with your Ollama API credentials:
     ```properties
     spring.application.name=ollamarestapi
     spring.ai.ollama.chat.model=mistral
     ```

## Running the Application

1. **Build the project**:
   ```sh
   ./gradlew clean build bootRun


## CREDITS
Raghu The Security Expert and ASG
