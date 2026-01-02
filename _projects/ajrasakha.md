---
layout: project
title: Ajrasakha
order: 5
summary: AI-powered agricultural advisory platform with expert knowledge base and multi-level review system
---


## Project Overview

Ajrasakha is an intelligent agricultural advisory platform that connects farmers with verified agricultural knowledge through an AI-powered chat interface. The system leverages a comprehensive Golden Dataset of verified agricultural Q&As and Package of Practices (PoP), using vector search and semantic similarity to provide accurate, context-aware answers. When the AI cannot find relevant information, questions are automatically routed to a network of agricultural experts for human review. The platform features a sophisticated multi-level moderation system with expert performance tracking, reputation scores, and a continuous learning mechanism where verified answers are added back to the Golden Dataset.

## Key Features

### For Farmers
- **AI Chat Interface**: Natural language conversation for agricultural queries
- **State & Crop-Specific Answers**: Contextualized responses based on location and crops
- **Multi-Language Support**: Regional language capabilities for wider accessibility
- **Real-time Query Status**: Track question progress through the review system

### Knowledge Base
- **Golden Dataset**: Vector-indexed database of verified agricultural Q&As with semantic search
- **Package of Practices (PoP)**: Comprehensive agricultural guidelines and best practices
- **Vector Search**: MongoDB Atlas vector search using HuggingFace embeddings (BAAI/bge-large-en-v1.5)
- **Automatic Dataset Growth**: Approved expert answers automatically added to Golden Dataset

### Expert & Moderation System
- **Expert Network**: Agricultural specialists provide answers for complex queries
- **Multi-Level Review**: Expert answers reviewed and approved by moderators
- **Performance Tracking**: Reputation scores, incentives, and penalties for experts
- **Approval Workflow**: Structured process ensuring quality control

### Analytics Dashboard
- **Golden Dataset Analytics**: Track dataset growth with year/month/week/day views
- **Expert Performance Metrics**: Monitor expert contributions and quality
- **Question Status Overview**: View distribution across open, in-review, and closed states
- **Moderator Approval Rate**: Track moderation efficiency
- **Contribution Trends**: Analyze question sources (Ajrasakha AI vs. Expert submissions)

## Technologies Used

### Backend
- TypeScript, Express.js, Node.js
- MongoDB with Vector Search (MongoDB Atlas)
- InversifyJS (Dependency Injection)
- Firebase Authentication
- Sentry (Error monitoring)

### Frontend
- React with TypeScript
- TanStack Router (File-based routing)
- TanStack Query (React Query)
- Shadcn UI components
- Tailwind CSS

### AI/ML
- **LLM Models**: DeepSeek-R1 (70B), Qwen3 (1.7B), GPT-OSS (20B) via Ollama
- **Embeddings**: HuggingFace BAAI/bge-large-en-v1.5
- **Vector Database**: MongoDB Atlas with vector indexing
- **MCP Servers**: Model Context Protocol for structured data access

### Additional Services
- MCP (Model Context Protocol) tools for Golden Dataset and FAQ access
- Audio processing for voice queries
- Sarvam AI API integration

## System Architecture

### Query Processing Workflow

1. **User Query Submission**: Farmer asks question via chat interface
2. **Context Detection**: System identifies user's state and crop information
3. **Golden Dataset Search**: Vector search finds semantically similar Q&As
4. **PoP Search**: If no match, searches Package of Practices database
5. **Expert Routing**: If still no answer, question sent to agricultural experts
6. **Expert Response**: Multiple experts provide answers with metadata
7. **Moderator Review**: Moderators approve and select best answer
8. **Dataset Update**: Approved Q&A added to Golden Dataset
9. **Farmer Notification**: Answer delivered to farmer

### User Roles

- **Farmers**: Submit questions, receive answers
- **Experts**: Answer routed questions, earn reputation scores
- **Moderators**: Review and approve expert answers
- **Admins**: System management and oversight

## Data Structure

### Golden Dataset
- Question-Answer pairs with embeddings
- Metadata: State, crop, season, domain, agri specialist, sources
- Similarity scores for retrieval
- Verification status

### Expert Performance
- Reputation scores
- Incentive tracking
- Penalty tracking
- Response quality metrics

## Project Goals

1. Provide instant, accurate agricultural guidance to farmers using AI
2. Build and maintain comprehensive Golden Dataset of verified agricultural knowledge
3. Connect farmers with agricultural experts for complex queries
4. Implement quality control through multi-level moderation
5. Track and incentivize expert contributions
6. Enable state and crop-specific agricultural advice
7. Support regional languages for broader farmer reach
8. Create self-improving knowledge base through continuous expert contributions
9. Provide analytics and insights on agricultural query patterns

## GitHub Repository

[Ajrasakha](https://github.com/vicharanashala/ajrasakha)
