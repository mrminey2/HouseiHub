# Housie Hub - Modern Tambola Gaming Platform

## Overview

Housie Hub is a modern web application for playing Tambola (Housie/Bingo) games online. It's built as a full-stack application with a React frontend and Express backend, designed to provide real-time multiplayer gaming experiences with various game modes, tournaments, and social features. The application supports both private rooms for family/friends and public tournaments with prize pools.

## User Preferences

Preferred communication style: Simple, everyday language.

## Recent Changes

**January 6, 2025 - Part 6 Complete: Live Chat & Points System**
- **Live Chat System**: Added real-time chat box in all game modes with minimizable interface and message history
- **Points System**: Implemented comprehensive point rewards for various game actions across all modes
- **Point Rewards**: Drawing numbers (5 Classic, 3 Speed, 10 Tournament), adding tickets (20), chatting (1), winning (100)
- **Interactive Chat**: Real-time messaging with username display, timestamps, system announcements
- **Points Display**: Floating points counter showing current player score with Ko-fi design consistency
- **Chat Storage**: In-memory message storage with support for user messages, system messages, and announcements
- **Enhanced UX**: Chat minimizes to floating icon, automatic scroll to new messages, responsive design
- **Game Integration**: Chat and points seamlessly integrated into existing game interfaces without disruption
- **Data Schema**: Extended database schema with chat messages table and user points tracking
- **Multiple Users**: Support for different usernames across game modes (Player1, SpeedPlayer, TournamentPro)

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite for build tooling
- **UI Library**: Shadcn/ui components built on Radix UI primitives
- **Styling**: Tailwind CSS with custom Ko-fi inspired color scheme
- **State Management**: TanStack Query for server state and React hooks for local state
- **Routing**: Wouter for client-side routing
- **Development Tools**: Hot module replacement and runtime error overlay for Replit environment

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Architecture Pattern**: RESTful API with modular route structure
- **Storage Interface**: Abstract storage layer with in-memory implementation (designed for easy database integration)
- **Development Mode**: Vite middleware integration for seamless full-stack development

### Data Storage Design
- **ORM**: Drizzle ORM configured for PostgreSQL
- **Database Schema**: 
  - Users table with authentication fields
  - Game rooms with host management and player limits
  - Game participants with ticket tracking and win states
- **Migration System**: Drizzle Kit for schema migrations
- **Validation**: Zod schemas generated from database schema for type safety

### Component Architecture
- **Design System**: Comprehensive UI component library with consistent theming
- **Layout Components**: Modular sections (Hero, Features, Community, etc.) for landing page
- **Responsive Design**: Mobile-first approach with responsive breakpoints
- **Animation**: CSS transitions and hover effects for enhanced user experience

## External Dependencies

### Core Framework Dependencies
- **@neondatabase/serverless**: Serverless PostgreSQL driver for Neon database
- **drizzle-orm**: Type-safe ORM with PostgreSQL dialect
- **@tanstack/react-query**: Server state management and caching
- **express**: Web application framework for Node.js

### UI and Styling Dependencies  
- **@radix-ui/react-***: Unstyled, accessible UI primitives for complex components
- **tailwindcss**: Utility-first CSS framework
- **class-variance-authority**: Component variant system for consistent styling
- **lucide-react**: Feather-inspired icon library

### Development Tools
- **vite**: Fast build tool and development server
- **@replit/vite-plugin-***: Replit-specific plugins for development environment
- **typescript**: Static type checking
- **wouter**: Lightweight client-side router

### Form and Validation
- **react-hook-form**: Performant forms with minimal re-renders
- **@hookform/resolvers**: Validation resolvers for react-hook-form
- **zod**: Schema validation library integrated with database schemas

### Additional Features
- **date-fns**: Date manipulation utilities
- **nanoid**: Unique ID generation
- **cmdk**: Command palette component
- **embla-carousel-react**: Touch-friendly carousel component