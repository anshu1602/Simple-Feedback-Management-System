   
# Simple Feedback Management System

# Overview
This project is a simple feedback management system that allows users to submit feedback and view all feedback entries. The system consists of a backend built with Node.js, Express, and TypeScript, and a frontend built with React and TypeScript.

## Project Setup
### Backend

1. Navigate to the backend directory:
   ```bash
   cd feedback-management-system
   
2. Install dependencies:

   ```bash
   npm install

3. Start the server:

   ```bash
   npm run dev
### Logic and Approach
Express Server: An Express server is set up in src/index.ts to handle incoming requests.

TypeScript: TypeScript is used for type safety and better development experience.

In-Memory Storage: Feedback entries are stored in an in-memory array to keep the implementation simple.

Controllers and Routes: The project uses a clear separation of concerns with controllers handling the logic and routes defining the API endpoints:

   GET /feedback: Retrieves all feedback entries.
   
   POST /feedback: Submits new feedback.

### FeedbackController (src/controllers/feedbackController.ts)
getAllFeedback: Retrieves all feedback entries from the in-memory array.

submitFeedback: Adds a new feedback entry to the in-memory array.

### Frontend
1. Navigate to the frontend directory:

   ```bash
   cd client

2. Install dependencies:

   ```bash
   npm install

3. Start the React app:

   ```bash
   npm start

### Logic and Approach
React Application: A React application is set up to provide a user interface for submitting and viewing feedback.

TypeScript: TypeScript is used for type safety and better development experience.

Axios: Axios is used to handle API requests to the backend.

Components:
   
   FeedbackForm: A form component to submit new feedback.
   
   FeedbackList: A component to display all feedback entries.

### FeedbackForm Component (src/components/FeedbackForm.tsx)

Handles form submission and sends a POST request to the backend to submit feedback.

### FeedbackList Component (src/components/FeedbackList.tsx)

Fetches and displays all feedback entries by sending a GET request to the backend.

### Project Structure
Backend: Node.js with Express and TypeScript
Frontend: React with TypeScript
Endpoints:
GET /feedback: Retrieve all feedback entries
POST /feedback: Submit new feedback

### Conclusion
This project provides a simple yet effective feedback management system with a clear separation of concerns between the backend and frontend, ensuring maintainability and scalability.


### Notes
Feedback entries are stored in an in-memory data structure (array).
No external in-memory storage solutions are used.


   ```sql
   ### Additional Notes

   - The optional rate limit and infinite scrolling features can be added as enhancements.
   - Ensure your backend and frontend servers are running simultaneously for full functionality.

   With these steps, you should have a fully functioning Simple Feedback Management System.

