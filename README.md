# Exam Portal Application
## Overview
This is a React-based exam portal application built with TypeScript, featuring a modern full-stack architecture. The application allows users to register, login, take exams across different subjects (Web Development, AI, Data Science), and view their results. It uses shadcn/ui for the component library and Firebase for data storage.
**Recent Migration**: Successfully migrated from Replit Agent to Replit environment (July 22, 2025). All features are fully functional with proper Firebase integration.
## User Preferences
Preferred communication style: Simple, everyday language.
## System Architecture
The application follows a monorepo structure with clear separation between client-side and server-side code:
- **Frontend**: React with TypeScript, using Vite as the build tool
- **Backend**: Express.js server with TypeScript support
- **Database**: Firebase Firestore for data persistence
- **UI Framework**: shadcn/ui components with Radix UI primitives
- **Styling**: Tailwind CSS with custom design tokens
- **State Management**: React Query for server state, Context API for auth state
- **Routing**: Wouter for client-side routing
## Key Components
### Frontend Architecture
- **Component Library**: Comprehensive shadcn/ui setup with 30+ pre-built components
- **Authentication**: Context-based auth system with Firebase integration
- **Forms**: React Hook Form with Zod validation
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **Build System**: Vite with TypeScript and React plugins
### Backend Architecture
- **Server Framework**: Express.js with TypeScript
- **Database Integration**: Drizzle ORM configured for PostgreSQL (though currently using Firebase)
- **Storage Layer**: Abstracted storage interface with in-memory implementation for development
- **API Structure**: RESTful API with /api prefix routing
### Data Models
The application defines several key schemas using Zod:
- **User**: Authentication and profile information
- **Question**: Exam questions with multiple choice options
- **Subject**: Exam subjects with questions and metadata
- **UserScore**: Score tracking across different subjects
- **ExamAttempt**: Individual exam attempt records
