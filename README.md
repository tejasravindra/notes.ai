# Notes.ai

Welcome to Notes.ai, an intelligent note-taking application designed to enhance your productivity and streamline your note-taking experience. Utilizing the power of OpenAI, Pinecone, and several other cutting-edge technologies, Notes.ai offers a smart, efficient, and highly customizable platform for all your note-taking needs.

## Features

- **AI-Powered Chat**: Chat with Notes.ai about any of your notes.
- **Light and Dark Mode**: Personalize your note-taking experience with light mode and dark mode.
- **Secure Authentication**: Protect your notes with robust security features powered by Clerk.

## Tech Stack

- **[Next.js](https://nextjs.org/)**: The React framework for production.
- **[OpenAI](https://www.openai.com/)**: AI models for generating and summarizing content.
- **[Pinecone](https://www.pinecone.io/)**: Managed vector database for scalable, accurate search.
- **[MongoDB](https://www.mongodb.com/)**: Document-based database for flexible, scalable data storage.
- **[Shadcn UI](https://ui.shadcn.com/)**: Modern UI library for React.
- **[Clerk](https://clerk.com/)**: User management and authentication tailored for modern applications.

## Getting Started

### Prerequisites

Before you start, ensure you have the following installed:

- Node.js
- npm or yarn

### Installation

Clone the repository:

```bash
git clone https://github.com/yourgithub/notes.ai.git
cd notes.ai
```

```bash
npm install
# or
yarn install
```

### Environment Setup
Before running the application, you need to set up your environment variables. Create a `.env` file in the root directory of the project and add the following keys with appropriate values:
```env
# MongoDB URL 
DATABASE_URL=""

# Clerk Keys
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Clerk Routing URLs:
## The URL where users are redirected to sign in.
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
## The URL where users are redirected to sign up.
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
## The URL where users are redirected after successfully signing in.
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/notes
## The URL where users are redirected after successfully signing up.
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/notes

# OpenAI API Key
OPENAI_API_KEY=""

# Pinecone API Key
PINECONE_API_KEY="" 
```
#### MongoDB
* For DATABASE_URL, set up a new database on MongoDB and use the connection string provided.
#### Clerk
* For CLERK_SECRET_KEY & NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY, create a new application on Clerk and go to API Keys.
* Keep Clerk's routing URLs as is. These help manage the flow of user authentication and post-authentication navigation within the app.
#### OpenAI
* For OPENAI_API_KEY, obtain the key through your account on OpenAI Platform.
#### Pinecone
* For PINECONE_API_KEY, create a new vector database at Pinecone to obtain the API key.

### Running the Application

To run the app locally:
```bash
npm run dev
# or
yarn dev
```
Open http://localhost:3000 with your browser to see the result.

## Acknowledgements
* OpenAI Team for their support and APIs
* Pinecone for their powerful search solutions
* Clerk for secure and seamless authentication
* Shadcn UI for the elegant design system


Thank you for choosing Notes.ai - your smart companion for effective note-taking!
