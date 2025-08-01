# Video Management System (VMS)

A modern web-based video management system built with FastAPI backend and React TypeScript frontend for monitoring and managing multiple video streams.

##  Features

- **Multi-Camera Support**: Manage up to 10 camera streams with real-time monitoring
- **Video Streaming**: Direct video file streaming with proper MIME types
- **Alert System**: Defect detection and alert management with confidence scoring
- **AI Integration**: AI-powered video analysis with asset and defect detection
- **Model Summaries**: Real-time AI model performance monitoring
- **Modern UI**: Responsive Bootstrap-based interface with TypeScript
- **RESTful API**: FastAPI backend with comprehensive endpoints and auto-generated docs
- **CORS Support**: Cross-origin resource sharing for frontend integration


##  Technology Stack

### Backend
- **FastAPI 0.116.1**: Modern Python web framework with automatic API documentation
- **OpenCV 4.9.0.80**: Computer vision and video processing
- **NumPy 1.26.4**: Numerical computing for AI operations
- **Uvicorn 0.35.0**: ASGI server for high-performance async operations
- **Pydantic 2.11.7**: Data validation and settings management
- **Starlette 0.47.2**: ASGI toolkit for building async web services

### Frontend
- **React 18**: Modern React with hooks and concurrent features
- **TypeScript 4.4.2**: Type-safe JavaScript for better development experience
- **Bootstrap 5.3.7**: Responsive UI framework with modern components
- **React Scripts 5.0.1**: Development and build tools

##  Prerequisites

- Python 3.8+ (3.10+ recommended)
- Node.js 16+ (18+ recommended)
- npm or yarn
- Git for version control

##  Quick Start

### 1. Clone the Repository
```bash
git clone <repository-url>
cd vms
```

### 2. Backend Setup

```bash
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Start the backend server
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

The backend will be available at `http://localhost:8000`

### 3. Frontend Setup

```bash
cd frontend

# Install dependencies
npm install

# Start the development server
npm start
```

The frontend will be available at `http://localhost:3000`

##  API Documentation

Once the backend is running, you can access:
- **Interactive API Docs**: `http://localhost:8000/docs`
- **ReDoc Documentation**: `http://localhost:8000/redoc`

### Key API Endpoints

- `GET /api/videos/` - List all available videos
- `GET /api/videos/{video_id}/stream` - Stream specific video
- `GET /api/streams/` - Get active camera streams
- `GET /api/summaries/` - Get AI model summaries
- `GET /api/alerts/` - Get system alerts

##  Usage

1. **Access the Dashboard**: Open `http://localhost:3000` in your browser
2. **View Camera Streams**: Navigate to the streams section to see active cameras
3. **Monitor Alerts**: Check the alerts panel for any detected issues
4. **View AI Analysis**: Access model summaries for AI-powered insights

##  Configuration

### Backend Configuration
- Video files are stored in `backend/app/videos/`
- Supported formats: MP4
- CORS is configured for `http://localhost:3000`

### Frontend Configuration
- API proxy is configured to `http://127.0.0.1:8000`
- Bootstrap is included for styling

##  Development

### Backend Development
```bash
cd backend
# Activate virtual environment
venv\Scripts\activate  # Windows
# source venv/bin/activate  # macOS/Linux

# Run with auto-reload
uvicorn app.main:app --reload
```

### Frontend Development
```bash
cd frontend
npm start
```

### Running Tests
```bash
# Backend tests
cd backend
python -m pytest

# Frontend tests
cd frontend
npm test
```




## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

##  Support

For support and questions:
- Create an issue in the repository
- Check the API documentation at `http://localhost:8000/docs`
- Review the code comments for implementation details

## Future Enhancements

- [ ] Real-time video streaming with WebRTC
- [ ] Advanced AI defect detection
- [ ] User authentication and authorization
- [ ] Database integration for persistent storage
- [ ] Mobile responsive design improvements
- [ ] Video recording and playback features 