# OmniMind AI

**OmniMind AI** is a powerful and customizable AI assistant designed to manage daily tasks and support users in multitasking, communication, and planning. This AI assistant is self-aware and adapts based on user preferences and habits. It supports natural interaction through voice and visual cues and learns from user behavior to make better decisions.

## Table of Contents
- [Key Features](#key-features)
- [Technologies](#technologies)
- [Use Cases](#use-cases)
- [AI Provider Integration](#ai-provider-integration)
- [Secure Environment Variable Management](#secure-environment-variable-management)
- [Getting Started](#getting-started)
- [Best Practices](#best-practices)
- [License](#license)

## Key Features
- **Natural Interaction**: Communicate via voice (microphone) and visual cues (camera) to respond to commands, detect emotions, and learn from behavior.
- **Task Management**: Manage emails, calendars, and tasks. Send notifications and reminders for important events and deadlines.
- **Phone Management**: Filter incoming calls, handle spam, and take action during emergencies.
- **Multitasking**: Execute multiple tasks simultaneously with real-time notifications and workflow suggestions.
- **Customizable 3D Avatar**: Generate and personalize a visual avatar to create a unique interaction experience.
- **AI Provider Integration**: Support for multiple AI providers, including OpenAI, Anthropic Claude, Hugging Face, and Ollama, allowing seamless switching between providers.
- **Voice Control**: Interact with OmniMind AI using voice commands for hands-free operation.
- **Location Services & Maps**: Access real-time location data and integrate with Google Maps and Apple Maps for navigation and location-based tasks.
- **Android Auto Integration**: Seamlessly interact with OmniMind AI through your car's infotainment system, enabling safe and convenient access while driving.
- **Secure Environment Variable Management**: Manage sensitive `.env` variables securely via a protected admin interface behind a login system.

## Technologies
- **Frontend**:
  - React Native
  - React Three Fiber
  - Expo
  - @react-native-voice/voice
  - react-native-maps
  - Android Auto SDK

- **Backend**:
  - Node.js
  - Express.js
  - MongoDB
  - Firebase Firestore

- **DevOps**:
  - Docker
  - Kubernetes
  - GitHub Actions
  - Terraform/Ansible

- **AI & NLP**:
  - OpenAI GPT-4
  - Anthropic Claude
  - Hugging Face Transformers
  - Ollama

- **Additional Tools**:
  - face-api.js / TensorFlow.js
  - Firebase Cloud Messaging (FCM)
  - LIME & SHAP
  - AIF360 & Fairness Indicators

## Use Cases
- **Daily Assistance**: Manage tasks and reminders, organize emails and calendars, and handle phone calls.
- **Emergency Handling**: Recognizes emergencies and can automatically contact emergency services or predefined contacts.
- **Learning Capability**: Learns from user interactions over time, adapting to provide better recommendations and actions.
- **Hands-Free Operation**: Control the assistant using voice commands without manual interaction.
- **Navigation & Location-Based Tasks**: Get directions, find nearby places, and receive location-specific reminders.
- **In-Car Assistance**: Access AI functionalities through Android Auto for safe, hands-free interaction while driving.

## AI Provider Integration
OmniMind AI integrates with multiple AI providers to leverage diverse NLP and conversational capabilities:
- **OpenAI**: General-purpose conversational AI and NLP tasks.
- **Anthropic Claude**: Context-rich responses and advanced NLP models.
- **Hugging Face**: Customizable models and open-source NLP solutions.
- **Ollama**: Domain-specific NLP tasks with advanced model support.

Users can select their preferred AI provider, input necessary API keys, and switch between providers based on specific tasks or desired performance.

## Secure Environment Variable Management
OmniMind AI securely manages environment variables by storing them in a database and restricting access through a protected admin interface. This ensures that sensitive information, such as API keys and configuration details, remains secure and is not exposed in the frontend or version control systems.

### Features:
- **Encrypted Storage**: Environment variables are encrypted before being stored in the database.
- **Admin Interface**: Accessible only to authenticated users with admin privileges for managing `.env` variables.
- **Role-Based Access Control (RBAC)**: Defines roles and permissions to control access to environment variables.
- **Audit Logging**: Tracks changes to environment variables for accountability and monitoring.

## Getting Started

### Prerequisites
- **Node.js** and **npm** installed
- **React Native CLI** or **Expo CLI**
- **MongoDB** instance
- **Firebase** project setup for Firestore and Authentication
- **Docker** and **Kubernetes** (optional for containerization)
- **Android Studio** for Android Auto Integration

### Installation
1. **Clone the repository**:
    ```bash
    git clone https://github.com/mupoese/OmniMind-AI.git
    cd OmniMind-AI
    ```

2. **Install Backend Dependencies**:
    ```bash
    cd backend
    npm install
    ```

3. **Install Frontend Dependencies**:
    ```bash
    cd ../frontend
    npm install
    ```

4. **Configure Environment Variables**:
    - Use the `backend/.env.example` as a template.
    - Store sensitive variables securely using the admin interface.

5. **Run the Backend Server**:
    ```bash
    cd backend
    npm start
    ```

6. **Run the Frontend Application**:
    ```bash
    cd ../frontend
    npm start
    ```

### Deployment
- **Docker**: Use Dockerfiles in the `docker/` directory to containerize the application.
- **Kubernetes**: Deploy using manifest files in the `k8s/` directory for orchestration.

## Best Practices
- **Security**:
  - Encrypt sensitive data stored in the database.
  - Implement role-based access control for the admin interface.
  - Regularly update dependencies to patch vulnerabilities.

- **Documentation**:
  - Maintain comprehensive documentation in the `docs/` directory.
  - Keep the `README.md` up-to-date with the latest features and setup instructions.

- **Code Quality**:
  - Use ESLint and Prettier for consistent code formatting and linting.
  - Implement thorough testing for all features to ensure reliability.

- **Deployment**:
  - Utilize CI/CD pipelines via GitHub Actions for automated testing and deployment.
  - Containerize applications with Docker and manage deployments with Kubernetes for scalability.

## License
This project is licensed under the [LICENSE.md](./LICENSE.md). Please review the license before using the software.
