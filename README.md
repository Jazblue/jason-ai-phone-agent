# Jason AI Phone Agent

AI-powered voice support prototype using Vapi and Twilio

## Overview

The Jason AI Phone Agent is an AI-powered voice support system designed to handle inbound and outbound phone calls with natural, conversational AI. Built using Vapi for AI voice orchestration and Twilio for telephony infrastructure, this project demonstrates real telephone calling functionality with a UK number. AWS backend services (Lambda, API Gateway, DynamoDB) are planned for future integration to enable call logging, automation, and scaling.

## Features

### Implemented
- AI-powered conversational voice agent
- Vapi integration for voice orchestration (assistant: `Jason AI Support`)
- Twilio for telephony (UK phone number)
- Real inbound and outbound telephone calls tested and verified
- Browser-based voice testing completed
- Clear, natural conversational interaction verified
- Security-first approach with no hardcoded credentials
- Modular design for extensibility

### Planned
- AWS backend integration (Lambda, API Gateway, DynamoDB)
- Call logging and records storage
- Calendar integration for scheduling
- Human escalation workflow
- Automated call summaries
- Monitoring and analytics

## Architecture

The current implemented flow connects the user to the AI assistant via Twilio and Vapi. Planned AWS integrations extend the system for data processing and automation.

```mermaid
flowchart LR
    A[User] --> B["Twilio UK Phone Number (redacted)"]
    B --> C[Vapi]
    C --> D[Jason AI Support Assistant]
    style A fill:#e8f4fd,stroke:#3498db,stroke-width:2px
    style B fill:#e8f4fd,stroke:#3498db,stroke-width:2px
    style C fill:#e8f4fd,stroke:#3498db,stroke-width:2px
    style D fill:#e8f4fd,stroke:#3498db,stroke-width:2px
    %% Planned components (dashed outline)
    E[Webhook/API] --> F[AWS API Gateway]
    F --> G[AWS Lambda]
    G --> H[DynamoDB / Calendar / Automation]
    style E fill:#f9e79f,stroke:#f39c12,stroke-width:2px,stroke-dasharray: 5 5
    style F fill:#f9e79f,stroke:#f39c12,stroke-width:2px,stroke-dasharray: 5 5
    style G fill:#f9e79f,stroke:#f39c12,stroke-width:2px,stroke-dasharray: 5 5
    style H fill:#f9e79f,stroke:#f39c12,stroke-width:2px,stroke-dasharray: 5 5
    %% Link from assistant to webhook (planned)
    D --> E
```

*Solid components: implemented and tested. Dashed components: planned future integrations.*

## Technology Stack

- **Vapi** – AI voice agent platform
- **Twilio** – Programmable SMS & Voice, UK phone number
- **Webhooks** – Event-driven integrations (planned)
- **AWS** – Backend services (planned)
  - Lambda – Serverless compute
  - API Gateway – HTTPS endpoints
  - DynamoDB – NoSQL database
- **AI Voice** – Large language model powered voice

## Current Status

### Completed
- Vapi assistant created (`Jason AI Support`)
- Browser voice test completed
- Voice conversation quality verified (user feedback: "really clear")
- Twilio account configured
- UK number selected ([UK number])
- Regulatory bundle submitted and approved (Twilio regulatory approval complete)
- Twilio UK number connected to Vapi assistant
- Real inbound telephone test successful (from mobile to Jason AI Support via Twilio number)
- Real outbound telephone test successful (from Jason AI Support to mobile phone)
- Both inbound and outbound real telephone calls connected successfully and allowed conversation with the AI assistant

### Planned
- AWS backend integration
- Call logging
- DynamoDB for call records
- Calendar integration for scheduling
- Human escalation workflow
- Automated call summaries
- Monitoring and analytics

## Setup

As this is a portfolio project demonstrating concept and architecture, there is no deployable code yet. Future implementation will require:

1. Vapi account and assistant configuration
2. Twilio account with approved UK number
3. AWS account with Lambda, API Gateway, and DynamoDB
4. Environment variables for all API keys and credentials
5. Webhook endpoints to connect Twilio → Vapi → AWS

## Security

- Never commit Twilio Auth Tokens or API keys to GitHub
- Never expose AWS access keys or secrets in client-side code
- Use environment variables and secrets management (GitHub Secrets, AWS Secrets Manager)
- Keep production credentials outside the public repository
- Validate and sanitize all webhook inputs
- Implement rate limiting and authentication for webhooks
- Follow principle of least privilege for IAM roles

## Future Roadmap

- Real-time call transcription and sentiment analysis
- Multi-language support
- Integration with CRM systems (Salesforce, HubSpot)
- Advanced call routing based on caller intent
- Voice biometrics for caller verification
- A/B testing of voice models and conversation flows
- Comprehensive logging and audit trails
- Load testing and scalability optimization

## Demo and Screenshots

The Vapi assistant "Jason AI Support" has been successfully tested through Vapi's browser voice interface, confirming clear, natural conversational interaction. Real telephone calls have been placed and received using the Twilio UK number, demonstrating end-to-end functionality.

*(Placeholder for future screenshots of Vapi assistant configuration, Twilio dashboard, and call logs.)*

## Author

Jason Harvey – AWS Cloud Engineer aspirant  
Chatham, Kent, UK  
GitHub: [@Jazblue](https://github.com/Jazblue)

## License

This project is proprietary and intended for portfolio purposes only.

## Acknowledgments

- Vapi for AI voice platform
- Twilio for telecommunications infrastructure
- AWS for cloud services
