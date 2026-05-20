# GoaTourWala - Backend

The backend API server for the GoaTourWala platform, built with Node.js, Express, and MongoDB.

## Features
- RESTful APIs for Categories, Subcategories, and Custom Planned Trips
- PhonePe Payment Gateway Integration
- Cloudinary Integration for Media Uploads
- Nodemailer for Automated Email Notifications

## Getting Started

### Prerequisites
- Node.js installed on your machine
- MongoDB Database (Local or MongoDB Atlas)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/gitCommit-Suryansh/goatourwala-backend.git
   ```
2. Navigate to the directory and install dependencies:
   ```bash
   cd goatourwala-backend
   npm install
   ```
3. Set up environment variables. Create a `.env` file in the root directory and add the necessary secrets:
   ```env
   PORT=5000
   # Database
   MONGO_URI=your_mongodb_connection_string
   
   # Cloudinary
   CLOUD_NAME=your_cloud_name
   API_KEY=your_api_key
   API_SECRET=your_api_secret

   # PhonePe Payment Gateway
   MERCHANT_ID=your_merchant_id
   SALT_KEY=your_salt_key
   CREATE_PAYMENT_URL=https://api.phonepe.com/apis/hermes
   CREATE_PAYMENT_ENDPOINT=/pg/v1/pay
   ```

### Running Locally
To start the server, run:
```bash
npm start
```
*(If you have `nodemon` installed for development, you can use `npm run dev`)*

The server will run on the port specified in your `.env` file (default is `5000`).
