# Jason AI Phone Agent

AI-powered voice support using Vapi, Twilio and AWS

## Overview

The Jason AI Phone Agent is an AI-powered voice support system designed to handle inbound and outbound phone calls with natural, conversational AI. Built using Vapi for AI voice orchestration, Twilio for telephony infrastructure, and planned AWS backend services for data processing and automation, this project aims to demonstrate a production-ready AI telephone agent prototype.

## Features

- AI-powered conversational voice agent
- Vapi integration for voice orchestration
- Twilio for telephony (UK number +44 1494 302460)
- Planned AWS backend (Lambda, API Gateway, DynamoDB)
- Browser-based voice testing completed
- Clear, natural conversational interaction verified
- Security-first approach with no hardcoded credentials
- Modular architecture for easy extensibility

## Architecture

```mermaid
flowchart LR
    A[User] --> B[Twilio UK Phone Number<br/>+44 1494 302460]
    B --> C[Vapi]
    C --> D[Jason AI Support Assistant]
    D --> E[Webhook/API]
    E --> F[AWS API Gateway]
    F --> G[AWS Lambda]
    G --> H[DynamoDB / Calendar / Automation]
```

*Components in red are planned future integrations.*

## Technology Stack

- **Vapi** – AI voice agent platform
- **Twilio** – Programmable SMS & Voice, UK phone number
- **AWS** – Backend services (planned)
- **Lambda** – Serverless compute (planned)
- **API Gateway** – HTTPS endpoints (planned)
- **DynamoDB** – NoSQL database (planned)
- **Webhooks** – Event-driven integrations
- **AI Voice** – Large language model powered voice

## Current Status

### Completed
October 2026 milestone  Real telephone calling verified
Jason AI Support has now successfully completed both inbound and outbound real telephone calls using Vapi and Twilio. The assistant can receive calls from a mobile phone and can also initiate an outbound call to a mobile phone. Both directions were tested successfully with live conversation.
- Vapi assistant created (`Jason AI Support`)
- Browser voice test completed
- Voice conversation quality verified (user feedback: "really clear")
- Twilio account configured
- UK number selected (+44 1494 302460)
- Regulatory bundle submitted and approved (Twilio regulatory approval complete)
- Twilio UK number connected to Vapi assistant
- Real inbound telephone test successful (from mobile to Jason AI Support via Twilio number)
- Real outbound telephone test successful (from Jason AI Support to mobile phone)
- Both inbound and outbound real telephone calls connected successfully and allowed conversation with the AI assistant

### Pending
- (All pending telephone tests completed)

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

## Screenshots / Demo

*(Placeholder for future screenshots of Vapi assistant configuration, Twilio dashboard, and AWS architecture diagrams)*

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
