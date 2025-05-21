# flight-booking-portal

# ✈️ Flight Booking System Using AWS

A simple web-based flight booking system built with HTML, CSS, and JavaScript. The backend is powered by AWS services including Lambda, DynamoDB, and API Gateway. The frontend is hosted on AWS S3.

## 🔧 Project Structure

📁 flight-booking-portal/
│
├── index.html # Homepage with hero banner
├── schedule.html # Flight schedule listing
├── book.html # Booking form that integrates with API Gateway + Lambda
├── thankyou.html # Thank you confirmation page after booking


## 🌐 Hosted Live Site

Your site is deployed and accessible here:

👉 [http://flight-booking-portal.s3-website-us-east-1.amazonaws.com](http://flight-booking-portal.s3-website-us-east-1.amazonaws.com)

> Replace with your actual S3 Bucket website endpoint if it differs.

---

## 🚀 Features

- User can view available flights.
- Users can fill in booking information (name, email, flight).
- Data is submitted via API Gateway → Lambda → DynamoDB.
- Confirmation message on successful booking.

---

## 📁 How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/flight-booking-portal.git
   cd flight-booking-portal
   
2. Host with AWS S3

   Create an S3 bucket (must be globally unique).

   Enable static website hosting.

   Upload all four .html files.

   Set index.html as the index document.

   Make the bucket contents public or use a CloudFront distribution.

3. API Integration

   Replace the API_URL in book.html with your actual API Gateway endpoint:
   const API_URL = "https://your-api-id.execute-api.us-east-1.amazonaws.com/flightbooking";


🔐 AWS Services Used
Amazon S3: Hosting static website (HTML/CSS/JS)

AWS Lambda: Executes booking logic

API Gateway (HTTP API): Accepts booking data from frontend

Amazon DynamoDB: Stores booking data

🙌 Credits
Built as part of a cloud project to demonstrate AWS serverless architecture.
