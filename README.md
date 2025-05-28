# AWS Amplify React+Vite Todo App Starter

![AWS Amplify](https://img.shields.io/badge/AWS%20Amplify-FF9900?style=for-the-badge&logo=aws-amplify&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

A modern, production-ready starter template for building full-stack applications using React, Vite, TypeScript, and AWS Amplify. This template includes a simple Todo application demonstrating authentication, real-time data, and cloud deployment capabilities.

## 📋 Overview

This template provides a fully configured development environment with:

- **Frontend**: React 18 with TypeScript and Vite for fast development and optimized builds
- **Backend**: AWS Amplify Gen 2 for simplified cloud resource provisioning
- **Authentication**: Pre-configured Amazon Cognito with email sign-in
- **Data Layer**: GraphQL API powered by AWS AppSync with real-time subscriptions
- **Database**: Serverless DynamoDB for scalable data storage
- **Deployment**: Streamlined deployment to AWS cloud infrastructure

## ✨ Features

- **Authentication System**: Secure user authentication with Amazon Cognito
  - Email-based login flow
  - Protected routes and authenticated API access
  
- **Real-time Todo Application**:
  - Create and view todos
  - Real-time updates using GraphQL subscriptions
  - Public API key authorization for demonstration purposes
  
- **Developer Experience**:
  - TypeScript for type safety and better developer experience
  - Fast refresh with Vite
  - AWS Amplify CLI integration for backend management
  - Clean project structure following best practices

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or later)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [AWS Account](https://aws.amazon.com/)
- [AWS Amplify CLI](https://docs.amplify.aws/cli/start/install/)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/amplify-vite-react-template.git
   cd amplify-vite-react-template
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn
   ```

3. Initialize Amplify:
   ```bash
   npx amplify init
   ```

4. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open your browser and navigate to `http://localhost:5173`

## 🏗️ Project Structure

```
/
├── amplify/               # AWS Amplify backend configuration
│   ├── auth/              # Authentication configuration
│   ├── data/              # Data models and GraphQL schema
│   └── backend.ts         # Backend definition
├── public/                # Static assets
├── src/
│   ├── assets/            # Frontend assets
│   ├── App.tsx            # Main application component
│   ├── App.css            # Application styles
│   └── main.tsx           # Application entry point
└── package.json           # Project dependencies and scripts
```

## 🔄 Development Workflow

1. **Local Development**:
   ```bash
   npm run dev
   ```

2. **Making Backend Changes**:
   - Edit files in the `amplify` directory
   - Run `npx amplify push` to deploy changes to the cloud

3. **Building for Production**:
   ```bash
   npm run build
   ```

4. **Preview Production Build**:
   ```bash
   npm run preview
   ```

## 📦 Deploying to AWS

1. Configure your AWS credentials:
   ```bash
   npx amplify configure
   ```

2. Deploy your application:
   ```bash
   npx amplify push
   ```

3. Deploy the frontend:
   ```bash
   npx amplify publish
   ```

For detailed deployment instructions, refer to the [AWS Amplify documentation](https://docs.amplify.aws/react/start/quickstart/#deploy-a-fullstack-app-to-aws).

## 🛠️ Customization

### Adding New Data Models

1. Edit `amplify/data/resource.ts` to add new models
2. Run `npx amplify push` to update your backend

### Modifying Authentication

1. Edit `amplify/auth/resource.ts` to change authentication settings
2. Run `npx amplify push` to update your backend

## 🔒 Security

This template uses public API keys for demonstration purposes. For production applications, consider implementing proper authentication and authorization rules.

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information on reporting security issues.

## 📄 License

This project is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file for details.