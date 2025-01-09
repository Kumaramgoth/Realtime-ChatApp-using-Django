# Realtime-ChatApp-using-Django

Overview
This is a real-time chat application built using Django Channels and WebSockets. The app allows users to:

Register and log in with an authentication system.
Join chat rooms and communicate with other users in real-time.
Utilize a user-friendly interface for seamless interaction.

Features
User Authentication:

Register, log in, and log out functionality using Django's built-in authentication system.
Real-Time Messaging:

WebSockets, powered by Django Channels, enable real-time communication between users.
Chat Rooms:

Create and join multiple chat rooms.
Send and receive messages in real-time within rooms.
Responsive UI:

Designed to be fully responsive with Bootstrap for an optimal experience on desktop and mobile.
Scalable:

Uses Redis to handle message broadcasting efficiently (using Django Channels).
Technologies Used
Backend:

Django
Django Channels
WebSockets
Redis (for message broadcasting)
Frontend:

HTML/CSS
JavaScript (for handling WebSocket connections)
Bootstrap (for responsive design)
Database:

SQLite (default; can be switched to PostgreSQL or MySQL for production)

Project Structure
graphql
Copy code
chat-app-django/
├── chat/                    # Main chat app
│   ├── templates/           # HTML templates for views
│   ├── consumers.py         # WebSocket Consumers for real-time messaging
│   ├── models.py            # Models for users, messages, chat rooms
│   ├── urls.py              # URL routing for the chat app
├── vchatapp/                # Project settings
│   ├── settings.py          # Django project settings
│   ├── asgi.py              # ASGI config for Django Channels
│   └── urls.py              # Project-wide URL routing
├── static/                  # Static files (CSS, JS, etc.)
├── db.sqlite3               # SQLite database (default)
├── requirements.txt         # Project dependencies
└── manage.py                # Django's management script
Key Files
asgi.py: Configures ASGI to handle WebSocket connections.
consumers.py: Defines the WebSocket consumers for real-time messaging.
models.py: Defines the database models for users, messages, and chat rooms.
settings.py: Django settings for database, channels, and other configurations.
urls.py: Project and app-specific routing.
![Screenshot 2025-01-09 200446](https://github.com/user-attachments/assets/b8f38e2f-140b-440b-a71a-d5ca0dae5b11)
![Screenshot 2025-01-09 200348](https://github.com/user-attachments/assets/0777dce3-56a3-4272-a975-07fef625bfea)
![Screenshot 2025-01-09 200717](https://github.com/user-attachments/assets/4118ee9b-5f5c-4c7a-80fc-fa60f8f6de5e)
![Screenshot 2025-01-09 200511](https://github.com/user-attachments/assets/edef932e-4587-4a44-946c-157b89960d27)

