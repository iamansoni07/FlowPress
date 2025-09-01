# FlowPress

A modern, feature-rich blog application built with Django and React, designed for content creators and bloggers.

## ✨ Features

- **User Management**: Complete authentication system with JWT tokens
- **Blog Management**: Create, edit, and manage blog posts with rich text editor
- **Category System**: Organize posts with customizable categories
- **Comment System**: Interactive commenting with reply functionality
- **User Profiles**: Customizable user profiles with social media links
- **Responsive Design**: Mobile-first design that works on all devices
- **Admin Panel**: Powerful Django admin interface with Jazzmin theme
- **Search & Filtering**: Advanced search and category-based filtering
- **Bookmarking**: Save favorite posts for later reading
- **Notifications**: Real-time notification system

## 🚀 Tech Stack

### Backend
- **Django 4.2** - High-level Python web framework
- **Django REST Framework** - Powerful API development toolkit
- **SQLite** - Lightweight database (easily switchable to PostgreSQL/MySQL)
- **JWT Authentication** - Secure token-based authentication
- **CKEditor** - Rich text editing capabilities

### Frontend
- **React 18** - Modern JavaScript library for building user interfaces
- **Vite** - Fast build tool and development server
- **Bootstrap 5** - Responsive CSS framework
- **Axios** - Promise-based HTTP client
- **React Router** - Declarative routing for React

## 📁 Project Structure

```
FlowPress/
├── backend/                 # Django backend
│   ├── api/                # Main Django app
│   ├── backend/            # Django project settings
│   ├── templates/          # Email templates
│   └── requirements.txt    # Python dependencies
├── frontend/               # React frontend
│   ├── src/
│   │   ├── views/         # React components
│   │   ├── utils/         # Utility functions
│   │   ├── store/         # State management
│   │   └── plugin/        # Custom plugins
│   └── package.json       # Node.js dependencies
└── README.md              # This file
```

## 🛠️ Getting Started

### Prerequisites
- Python 3.8+
- Node.js 16+
- npm or yarn

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run migrations:
   ```bash
   python manage.py migrate
   ```

5. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```bash
   python manage.py runserver
   ```

The backend will be available at `http://localhost:8000`

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

The frontend will be available at `http://localhost:5173`

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the backend directory:
```env
SECRET_KEY=your-secret-key-here
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
FROM_EMAIL=your-email@example.com
```

### Database Configuration
The default configuration uses SQLite. To use PostgreSQL or MySQL, update the database settings in `backend/backend/settings.py`.

## 📱 API Documentation

Once the backend is running, you can access the interactive API documentation at:
- **Swagger UI**: `http://localhost:8000/`
- **Admin Panel**: `http://localhost:8000/admin/`

## 🎨 Customization

### Styling
- Modify Bootstrap variables in `frontend/src/index.css`
- Update component styles in individual component files
- Customize the Jazzmin admin theme in `backend/backend/settings.py`

### Features
- Add new models in `backend/api/models.py`
- Create new API endpoints in `backend/api/views.py`
- Build new React components in `frontend/src/views/`

## 🚀 Deployment

### Backend Deployment
1. Set `DEBUG=False` in production
2. Configure your production database
3. Set up static file serving
4. Use a production WSGI server like Gunicorn

### Frontend Deployment
1. Build the production version:
   ```bash
   npm run build
   ```
2. Deploy the `dist` folder to your web server

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with Django and React
- Styled with Bootstrap 5
- Admin theme by Jazzmin
- Icons by Font Awesome and Bootstrap Icons

## 👨‍💻 Developer

**FlowPress** is developed and maintained by:

- **Name**: Aman Soni
- **Email**: [aman.soni0713@gmail.com](mailto:aman.soni0713@gmail.com)
- **Location**: Delhi, India
- **GitHub**: [iamansoni07](https://github.com/iamansoni07)

## 📞 Support

For support and questions:
- Create an issue on GitHub
- Email: [aman.soni0713@gmail.com](mailto:aman.soni0713@gmail.com)
- Check the documentation
- Review the code examples

---

**FlowPress** - Empowering content creators with a modern, flexible blogging platform.

*Developed with ❤️ by Aman Soni*
