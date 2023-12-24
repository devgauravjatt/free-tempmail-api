
# 📑 Temp Mail API Documentation

Effortlessly manage temporary email accounts and messages with the Temp Mail API. This user-friendly and efficient solution is ideal for applications, websites, or new projects with temporary email services. 📧✨

## 📝 How to Get Started?

Getting started is simple with the Temp Mail API:

**😎 API Base URL:** `https://free-tempmail-api.vercel.app/api/`

### 1. 📨 Get New Mail Account
- **Endpoint:** `/newmail`
- **Method:** GET
- **Description:** Create a new temporary email account.
- **Query Parameters:** None
- **Example Request:**
  ```
  GET /newmail
  ```
- **Example Response:**
  ```json
  {
    "success": true,
    "newmail": {
      "email": "susan119776@hldrive.com",
      "token": " your token hare "
    }
  }
  ```


### 2. 📩 Get All Mail
- **Endpoint:** `/mails`
- **Method:** GET
- **Description:** Retrieve all emails in the temporary mailbox.
- **Query Parameters:** None
- **Headers:** 
  - `mailtoken` (string, required): The authentication token for accessing the mailbox.
- **Example Request:**
  ```
  GET /mails
  Headers:
    mailtoken: your_token_here
  ```
- **Example Response:**
  ```json
  {
    "success": true,
    "mails": [{ get all mails here }]
  }
  ```

### 3. 📖 Read Mail by ID
- **Endpoint:** `/read/{mail_id}`
- **Method:** GET
- **Description:** Read a specific email in the temporary mailbox by its ID.
- **Path Parameters:**
  - `mail_id` (string, required): The unique identifier of the email.
- **Example Request:**
  ```http
  GET /read/658839bc9995d8263956db24
  ```
- **Example Response:**
  ```json
  {
    "success": true,
    "mail": {
      "id": "658839bc9995d8263956db24",
      "seen": true,
      "from": {
        "address": "devgdjatt@onmail.com",
        "name": "Nina Mejia"
      },
      "to": [
        {
          "address": "longdyane@desertsundesigns.com",
          "name": ""
        }
      ],
      "cc": [],
      "bcc": [],
      "subject": "",
      "text": "your mail text here",
      "html": [
        "<div>your mail text here</div>"
      ],
      "date": "2023-12-24T14:01:24+00:00"
    }
  }
  ```

#


Begin your journey with the Temp Mail API today and experience the convenience of managing temporary email accounts effortlessly! 📧✨

## 🎉 Credits
We want to acknowledge and appreciate the hard work and creativity of our development team. They've made this API a reality. 🙌

- Lead Developer: [**Dev. Gaurav Jatt 👨‍💻**](https://github.com/devgauravjatt)
- Backend Developer: [**Dev. Gaurav Jatt 👨‍💻**](https://github.com/devgauravjatt)
#
