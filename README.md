# AWS QR based feedback system
Our objective in this project is to increase tenant satisfaction and operational efficiency
by using Amazon Web Services (AWS) and Quick Response (QR) codes.

Our endeavor revolves around implementing a feedback mechanism accessible by QR
codes that exists in various amenities within a residential building, such as trash bins, elevators,
storage rooms and so on. These QR codes are used as gateways to connect tenants to our
feedback platform.

This feedback process begins with tenants scanning the QR code with the amenity they
wish to give feedback on. After scanning, they are redirected to a web interface, urging them to
register themselves then log in. Registration requires a unique user name and a password which
is stored in MySQL database.

Once authenticated, tenants can access the feedback submission form. This feedback then
is forwarded to the administrator.
### Feedback Submission Process
1. Scanning the QR Code: Tenants scan the QR code on the specific amenity they wish to give
feedback on.
2. Redirect to Web Interface: The QR code redirects the tenant to a web interface where they are
prompted to register or log in.
3. Feedback Form Access: Upon successful authentication, tenants can access the feedback
submission form tailored to the specific amenity.
4. Form Submission: Tenants fill out the feedback form, which includes fields for rating, comments,
and suggestions.

## Usage Concepts
### 1 - AWS EC2 
We write a flask application and run with Aws EC2 (ubuntu).
### 2 - AWS RDS
For the database we used the Aws RDS postresql.
### 3 - AWS S3 
For creating and keeping qr datas we are using Aws S3

## important libraries
### 1 - nginx
For web server software we used nginx library.
### 2 - gunicorn
We used this library to run our Python flask application simultaneously by running multiple Python processes on a single dyno.

 
 
