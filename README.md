# **Python Application**

This project provides a Python-based API application using **FastAPI**. Follow the steps below to set up and run the project locally.

---

## **Prerequisites**
Before proceeding, ensure that you have the following installed on your system:

- **Python** (>=3.8)
- **pip** (Python package manager)
- **Git**

---

## **Setup Instructions**

### **1. Clone the Repository**
To get started, clone this repository to your local machine using the following command:

```bash
git clone <repository-url>
```

### **2. Navigate to the Project Directory**
Go to the project directory where the repository is cloned:

```bash
cd <repository-folder>
```

### **3. Install Dependencies**
Install the required Python packages using `pip`:

```bash
pip install -r requirements.txt
```

### **Configuration Files**
The following configuration files are required for the application:

- **.env**: Contains sensitive environment variables, like API keys or database credentials.
    - You need to create a `.env` file in the project root and add your OpenAI API key like so:
    ```env
    OPENAI_APIKEY=your-openai-api-key
    ```
---

### **Environment Variables**
The application uses the following environment variables:
- `OPENAI_APIKEY`: Your OpenAI API key to access OpenAI's services.

Make sure you have set these variables correctly in the `.env` file before starting the application.


### **Run the Application**
Start the FastAPI application locally using the `uvicorn` server:

```bash
python -m uvicorn main:app --reload
```


## **API Endpoints**

Below are the available API endpoints and their descriptions:

---

### **1. Predict**
- **Endpoint**: `POST /predict`
- **Path**: `routes/predict.py`
- **Description**: Handles predictions based on the provided input.

---

### **2. Train and Test**
- **Endpoints**:
  - `POST /train_and_test`: Trains and tests the model.
  - `GET /`: Returns metadata or status.
- **Path**: `routes/model.py`

---

### **3. Get Players**
- **Endpoint**: `GET /players`
- **Path**: `routes/getplayers.py`
- **Description**: Fetches details of players.

---

### **4. Get Unique Teams**
- **Endpoint**: `GET /unique_teams`
- **Path**: `routes/getteams.py`
- **Description**: Returns a list of unique teams.

---

### **5. Chatbot**
- **Endpoint**: `POST /chatbot`
- **Path**: `routes/chatbot.py`
- **Description**: Handles chatbot interactions.


## **Project Structure**
The application follows a modular structure:

bash
```
project-root/
│
├── main.py                # Entry point of the application
├── routes/                # Contains all route modules
│   ├── predict.py
│   ├── model.py
│   ├── getplayers.py
│   ├── getteams.py
│   ├── chatbot.py
│
├── requirements.txt       # Dependencies
├── README.md              # Documentation
└── ...

```


#   Steps to Run  Project on Localhost

## 1\. Clone the Repository

Clone the repository using the following command:

```
git clone <repository-url>
```

Replace <repository-url> with the GitHub repository URL.

- - -

## 2\. Navigate to the Project Directory

After cloning the repository, move into the project folder:

```
cd <project-folder-name>
```

- - -

## 3\. Install Dependencies

Install the required Node.js dependencies.

### 3.1. Ensure Node.js and npm are Installed

Check the versions of Node.js and npm:

```
node -v
```

```
npm -v
```

**Note:** Recommended Node.js version is 16 or higher.

### 3.2. Install Dependencies

Run the following command to install dependencies:

```
npm install
```


- - -

## 4\. Run the Development Server

Start the Next.js development server with:

```
npm run dev
```
- - -

The application will be available at:

`http://localhost:3000`

- - -



## Summary

1.  Clone the repository: `git clone <repository-url>`
2.  Navigate to the project folder: `cd <project-folder-name>`
3.  Install dependencies: `npm install`
4.  Run the development server: `npm run dev`


This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
