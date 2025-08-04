# PST Gmail Converter

This project allows you to:
- Import emails from a PST file
- View, export, and send emails via Gmail
- Export emails as simple, readable PDFs 
---

## Prerequisites

- **Java 17+**
- **Node.js 16+** (for frontend)
- **Maven** (for backend)
- **Google Cloud Project** with Gmail API enabled

---

## Setup Instructions

###  Backend Setup

#### a. Install Dependencies

```sh
cd backend
mvn clean install
mvn clean install

mvn spring-boot:run
```
- The backend runs on [http://localhost:8081](http://localhost:8081) by default.
- On first run, a browser window will open for Google OAuth. Complete the login.

### 3. Frontend Setup

```sh
cd ../frontend
npm install
npm start
```

- The frontend runs on [http://localhost:3000](http://localhost:3000) by default.

---

## Usage

- **Import PST:** Upload your PST file in the frontend.
- after uploading the file you just need to refresh the page you will see your pst files 

- click on one of the pst files 
- you will able to see the email in that pst file

- **View Emails:** Click "View" to see email details.

- **Export as PDF:** Click "Export" to download a simple PDF of the email.

- **Send to Gmail:** Enter a recipient and click "Send" to send via Gmail.

- but before the send the gmail put credentials.json file in root directory where frontend backend and jar file is present 

- credentials.json file is present in the backend root directory copy and paste to root directory of the project 


- when you click to send email you just goto your code - editor there is link visible 
like this-
[ "https://accounts.google.com/o/oauth2/auth?access_type=offline&client_id=513717795676-hncig86csuelq70lbi6b0h7ftu73fth8.apps.googleusercontent.com&redirect_uri=http://localhost:8888/Callback&response_type=code&scope=https://www.googleapis.com/auth/gmail.send"]

copy that link and paste on the browser 

just signup (email id should be this akashsahu.blue@gmail.com) i have added your email in google console as test user so you can test the app.
to that link and return to react app
you will see a message like email sent 

check your given email address 

email has come by your email address to your recipent email address

- for filter 

- put the To's email address of your pst 
in the input box this will filter the email address.

- for sending bulk messages 
put the email address in recipent address all email wiill send to the recipent address

---

## Troubleshooting

- **Port already in use:**  
  Stop the process using the port or change the port in `backend/src/main/resources/application.properties` (`server.port=8082`).




# PST-to-Gmail-Converter
