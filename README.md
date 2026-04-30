# Abbas Agha - AI Financial Copilot

Abbas Agha is an AI-powered financial copilot built on top of the bunq banking API.

The goal of this project is to make banking feel more natural, helpful, and interactive by combining chat, financial insights, receipt analysis, and future voice assistant features.

This project started during the **bunq Hackathon 7.0 — Multimodal AI** challenge and is now being improved into a more complete fintech assistant.

---

## Project Vision

Modern banking apps are often good at showing numbers, but they are not always good at helping users understand their money.

Abbas Agha aims to act like a personal financial assistant that can:

- answer financial questions in natural language
- analyze transactions and spending behavior
- scan receipts and categorize expenses
- give proactive warnings about risky or unusual spending
- support voice-based banking commands
- connect with the bunq sandbox API for safe testing

The long-term goal is to build a multimodal AI assistant that can **read, listen, understand, and act**.

---

## Main Features

### Current Features

- AI financial copilot interface
- Chat-based assistant UI
- Backend structure for AI and banking logic
- bunq sandbox API integration foundation
- Project documentation and setup structure

### Planned Features

- Voice assistant for banking commands
- Receipt image upload and AI receipt analysis
- Transaction categorization
- Spending summary and budget insights
- Proactive financial warnings
- Improved dashboard UI
- Better authentication and user session handling
- More complete bunq API integration
- Tests for backend and frontend functionality

---

## Example Use Cases

A user should be able to ask:

```text
How much did I spend this week?
```

```text
Show my latest transactions.
```

```text
Scan this receipt and add it to my food expenses.
```

```text
Warn me if I spend too much on subscriptions.
```

```text
Send €10 to Alex.
```

For safety, real payment actions should first be tested only in the bunq sandbox environment.

---

## Tech Stack

### Frontend

- TypeScript
- JavaScript
- CSS
- Modern web UI structure

### Backend

- Python
- bunq API sandbox
- AI assistant logic
- REST API structure

### Tools

- Git
- GitHub
- VS Code
- bunq Developer API
- AI / multimodal model integrations

---

## Project Structure

```text
abbasagha/
├── backend/                 # Backend API and AI/banking logic
├── frontend/                # Frontend chat and dashboard UI
├── docs/                    # Extra documentation
├── .gitignore
├── README.md
├── folder_structure.txt
└── requirements.txt
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/kiarashdelavar/abbasagha.git
cd abbasagha
```

Or, if you are working from the original repository:

```bash
git clone https://github.com/MohammadRezaMortazavi/abbasagha.git
cd abbasagha
```

---

## Backend Setup

Go to the backend folder:

```bash
cd backend
```

Create and activate a virtual environment.

### Windows PowerShell

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r ../requirements.txt
```

Start the backend according to the backend entry file used in the project.

Example:

```bash
python main.py
```

If the backend uses another entry file, check the `backend/` folder and run the correct file.

---

## Frontend Setup

Open a new terminal and go to the frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend:

```bash
npm run dev
```

The frontend will usually run on:

```text
http://localhost:5173
```

or another port shown in the terminal.

---

## Environment Variables

Create a `.env` file when needed.

Example variables:

```env
BUNQ_API_KEY=your_bunq_sandbox_api_key_here
AI_API_KEY=your_ai_api_key_here
BACKEND_URL=http://localhost:8000
```

Never commit real API keys to GitHub.

---

## bunq Sandbox

This project should use the bunq sandbox for development and testing.

The sandbox allows testing with fake money and fake users, so no real money is used.

Useful bunq resources:

- [bunq API Documentation](https://doc.bunq.com)
- [bunq Developer Portal](https://developer.bunq.com)

---

## Development Workflow

This project should be improved using a clean Git workflow.

### 1. Update main

```bash
git checkout main
git pull origin main
```

### 2. Create a feature branch

```bash
git checkout -b feature/voice-assistant
```

### 3. Commit changes

```bash
git add .
git commit -m "feat: add voice assistant interface"
```

### 4. Push the branch

```bash
git push origin feature/voice-assistant
```

### 5. Open a Pull Request

Open a pull request on GitHub so the changes can be reviewed before merging.

---

## Suggested Branches

```text
feature/project-cleanup
feature/voice-assistant
feature/receipt-analysis
feature/financial-copilot-chat
feature/proactive-warnings
feature/bunq-api-integration
feature/ui-redesign
feature/backend-tests
```

---

## Roadmap

### Phase 1 — Project Cleanup

- Update README and branding
- Clean folder structure
- Add environment variable examples
- Improve setup instructions

### Phase 2 — AI Chat Improvements

- Improve chatbot prompts
- Add financial context handling
- Add better error messages
- Store conversation history

### Phase 3 — Multimodal Features

- Add voice input
- Add speech-to-text
- Add receipt image upload
- Extract merchant, date, total amount, and category from receipts

### Phase 4 — Banking Intelligence

- Connect to bunq sandbox transactions
- Summarize spending
- Categorize expenses
- Detect unusual spending
- Add budget warnings

### Phase 5 — Production Quality

- Add tests
- Improve security
- Improve UI/UX
- Add CI/CD checks
- Add deployment documentation

---

## Safety Notes

This project is for learning, experimentation, and sandbox testing.

Before enabling real financial actions:

- use sandbox mode first
- require user confirmation before payments
- never store API keys in the frontend
- never commit secrets
- validate all user actions
- log important actions safely
- protect payment-related endpoints

---

## Contributors

- [Kiarash Delavar](https://github.com/kiarashdelavar)
- [MohammadReza Mortazavi](https://github.com/MohammadRezaMortazavi)
- [Kourosh Delavar](https://github.com/Kourosh-Delavar)

---

## License

No license has been added yet.

Before using this project commercially or publicly, add a clear license file.
