# Python Chat App

A real-time web chat application built with Flask and Flask-SocketIO. Users are assigned temporary usernames and avatars when they connect, can exchange messages in real time, and can update their display name.

## Features

- Real-time messaging with WebSockets
- Automatic temporary username generation
- Random avatar assignment
- Join/leave notifications
- Username updates
- Browser-based chat UI using Flask templates

## Tech Stack

- Python
- Flask
- Flask-SocketIO
- HTML/CSS/JavaScript
- WebSockets

## Project Structure

```text
.
├── app.py
├── wsgi.py
├── requirements.txt
├── templates/
│   └── index.html
└── .gitignore
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/VCShekhar96/Python-Chat-App.git
cd Python-Chat-App
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

- Windows: `.venv\\Scripts\\activate`
- macOS/Linux: `source .venv/bin/activate`

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Then open the local address shown by Flask in your browser.

## Notes

User state is held in memory, so connected-user data is not intended to persist across restarts. The application also uses an external avatar service for generated avatar URLs.

## Future Improvements

- Persistent message storage
- Authentication and user accounts
- Input validation and rate limiting
- Private chat rooms
- Automated tests
- Production deployment configuration

## Security

Do not place passwords, API keys, session secrets, or other credentials directly in source files. Use environment variables for sensitive configuration as the project evolves.

## License

No license is currently declared. Add an explicit license if you intend others to reuse or distribute the project.
