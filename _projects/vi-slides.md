---
layout: project
title: Vi-SlideS
order: 6
summary: AI-powered adaptive classroom platform that tailors teaching based on student questions and cognitive analysis
---

## Project Overview

Vi-SlideS is an intelligent classroom interaction platform that revolutionizes teaching by making it question-driven and adaptive. After a brief 5-10 minute topic introduction, students submit questions that shape the direction of the class. The system uses AI to analyze the collective questions, providing teachers with real-time insights into class mood, motivation, and conceptual understanding. AI automatically addresses straightforward questions, allowing teachers to focus on complex, cognitively intensive queries that require deeper explanation and personalized attention.

## Key Features

### Student Interaction
- **Question Submission Interface**: Students ask questions after topic introduction
- **Real-time Question Collection**: Aggregate student queries during class
- **Anonymous or Identified Submissions**: Flexible submission options
- **Question Status Tracking**: See which questions are AI-answered vs. teacher-addressed

### AI-Powered Analysis
- **Class Mood Detection**: Analyze questions to gauge overall class sentiment
- **Motivation Assessment**: Understand student engagement and interest levels
- **Cognitive Level Classification**: Identify conceptual depth and complexity of questions
- **Gist Extraction**: Summarize main themes and concerns from all questions
- **Learning Gap Identification**: Detect common misconceptions or knowledge gaps

### Automated Response System
- **Smart Question Triage**: AI determines which questions can be auto-answered
- **Instant AI Responses**: Automatically answer straightforward, factual questions
- **Complexity Detection**: Route cognitively intensive questions to teacher
- **Uniqueness Filter**: Prioritize novel, thought-provoking questions for teacher
- **Reference Integration**: AI provides answers with relevant sources and examples

### Teacher Dashboard
- **Question Overview**: See all student questions in real-time
- **Class Insights Panel**: View mood, motivation, and knowledge gap analytics
- **Question Prioritization**: AI-ranked questions based on complexity and importance
- **Teaching Direction Guidance**: Suggested class flow based on question patterns
- **Response Review**: Monitor and override AI-generated answers if needed

## Technologies Used

### Current Testing Phase
- Google Forms (Question collection)
- Google Sheets (Data aggregation and analysis)
- Google Slides (Presentation and visualization)

### Planned Technology Stack for Development
- Frontend: React, TypeScript
- Backend: Express.js, Node.js
- Database: MongoDB
- AI/NLP: Large Language Models for question analysis and response generation
- Sentiment Analysis: NLP models for mood and motivation detection
- Classification Models: Cognitive complexity assessment algorithms
- Real-time Communication: WebSockets for live question updates

## System Workflow

### Pre-Class Phase
1. **Topic Introduction**: Teacher presents 5-10 minute overview of topic
2. **Question Collection**: Students submit questions through platform

### AI Analysis Phase
3. **Question Ingestion**: System collects all student questions
4. **Cognitive Analysis**: AI classifies questions by complexity and uniqueness
5. **Mood & Motivation Analysis**: System analyzes collective sentiment
6. **Gist Generation**: AI creates summary of class understanding and concerns

### Response Phase
7. **Auto-Response**: AI immediately answers straightforward questions
8. **Teacher Queue**: Complex questions routed to teacher dashboard
9. **Class Direction**: Teacher uses insights to guide class discussion
10. **Dynamic Adaptation**: Teacher addresses high-priority questions

### Post-Class Phase
11. **Analytics Report**: Comprehensive class engagement and learning report
12. **Question Archive**: Store Q&A for future reference

## Question Classification

### AI Auto-Answered Questions
- Factual or definition-based queries
- Previously answered similar questions
- Low cognitive complexity
- Standard clarifications

### Teacher-Addressed Questions
- High conceptual depth
- Novel perspectives or applications
- Complex problem-solving scenarios
- Questions requiring personalized explanation
- Critical thinking and analysis queries

## Project Goals

1. Transform traditional lectures into question-driven, adaptive learning experiences
2. Provide real-time insights into class understanding and engagement
3. Reduce teacher burden by automating straightforward question responses
4. Enable teachers to focus on complex, high-value discussions
5. Improve student engagement through responsive teaching
6. Identify learning gaps and misconceptions early
7. Create data-driven teaching strategies based on question analysis
8. Foster more interactive and student-centered classrooms

## GitHub Repository

[Vi-SlideS(TBD)](https://github.com/vicharanashala/)
