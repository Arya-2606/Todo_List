# Task Master Pro

A modern, interactive todo application built with Flask and featuring a beautiful Mercury Academy-inspired frontend design.

## 🚀 Features

### Core Functionality
- ✅ Add new tasks with a clean, intuitive interface
- ✅ Mark tasks as completed
- ✅ Delete tasks
- ✅ SQLite database for persistent storage
- ✅ Real-time task statistics

### Interactive Frontend
- 🎨 Modern, responsive design with glassmorphism effects
- 📱 Mobile-friendly interface
- 🔄 Smooth animations and micro-interactions
- 📊 Live statistics dashboard (Total, Completed, Pending tasks)
- 🔍 Filter tasks by status (All, Pending, Completed)
- ⚡ Interactive buttons with satisfying press effects
- 🎯 Floating action button for quick task addition
- 🌈 Beautiful gradient backgrounds and modern typography

### User Experience
- 💫 Smooth transitions and hover effects
- 📈 Animated statistics counters
- 🎪 Empty state illustrations
- 🖱️ Intuitive click and touch interactions
- 📱 Fully responsive design for all devices

## 🛠️ Tech Stack

- **Backend**: Flask 2.3.3
- **Database**: SQLite
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with modern design patterns
- **Icons**: Font Awesome 6.4.0
- **Fonts**: Google Fonts (Inter)

## 📋 Installation

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### Setup Instructions

1. **Clone or download the project**
   ```bash
   git clone <repository-url>
   cd todo_app
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

5. **Access the application**
   Open your web browser and navigate to `http://127.0.0.1:5000`

## 🏗️ Project Structure

```
todo_app/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
├── tasks.db             # SQLite database (auto-created)
└── templates/
    └── index.html       # Main HTML template with modern UI
```

## 🎮 Usage Guide

### Adding Tasks
1. Type your task in the input field labeled "What needs to be done today?"
2. Click the "Add Task" button or press Enter
3. Your task will appear in the list below

### Managing Tasks
- **Complete a task**: Click the green checkmark button
- **Delete a task**: Click the red trash button
- **Filter tasks**: Use the tabs to view All, Pending, or Completed tasks

### Interactive Features
- **Statistics**: View real-time task counts in the dashboard
- **Floating Action Button**: Click the + button in the bottom-right to quickly scroll to top and focus the input field
- **Hover Effects**: All interactive elements respond to mouse hover
- **Press Effects**: Buttons have satisfying press animations

## 🎨 Design Features

### Visual Elements
- **Modern Typography**: Clean Inter font family
- **Color Scheme**: Professional purple and blue gradients
- **Glassmorphism**: Subtle blur effects and transparency
- **Smooth Animations**: CSS transitions and keyframe animations
- **Responsive Grid**: Adapts to different screen sizes

### Interactions
- **Button Press Effects**: Realistic press animations with shadow changes
- **Task Animations**: Tasks slide in when added
- **Hover States**: All interactive elements respond to hover
- **Loading Animations**: Statistics counters animate on page load

## 🔧 Configuration

### Database
The application uses SQLite for data storage. The database file (`tasks.db`) is automatically created when you first run the application.

### Customization
You can customize the application by modifying:
- **Colors**: Edit CSS variables in `templates/index.html`
- **Fonts**: Change the Google Fonts import
- **Animations**: Modify CSS keyframes and transitions
- **Layout**: Adjust grid layouts and responsive breakpoints

## 📱 Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🚀 Deployment

### Local Development
```bash
python app.py
```

### Production Deployment
For production deployment, consider using a WSGI server like Gunicorn:

```bash
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:5000 app:app
```

### Docker Deployment
Create a `Dockerfile`:
```dockerfile
FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5000
CMD ["python", "app.py"]
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🐛 Troubleshooting

### Common Issues

**Port already in use:**
```bash
# Find the process using the port
netstat -ano | findstr :5000
# Kill the process
taskkill /PID <process-id> /F
```

**Database issues:**
- Delete `tasks.db` to reset the database
- The application will recreate it on next run

**Styling issues:**
- Ensure you have an internet connection for Google Fonts and Font Awesome
- Check browser console for any CSS errors

## 📞 Support

For support or questions:
- Create an issue in the repository
- Check the troubleshooting section above
- Review the code comments for additional context

---

**Built with ❤️ using Flask and modern web technologies**
