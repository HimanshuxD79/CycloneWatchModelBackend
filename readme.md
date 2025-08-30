# Cyclone Watch

Cyclone Watch is a machine learning-powered web application for predicting cyclone intensity from satellite images. Built with Django and TensorFlow, it provides a simple interface to upload images and receive predictions.

## Features

- Upload satellite images to predict cyclone intensity
- REST API support
- Admin dashboard (Django)
- Docker support for easy deployment

## Quick Start

### Requirements

- Python 3.11
- Django 4.2
- TensorFlow 2.12
- See `requirements.txt` for full dependencies

### Setup & Run

Clone the repository and install dependencies:

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Or use Docker:

```bash
docker build -t cyclone-watch .
docker run -p 8000:8000 cyclone-watch
```

Access the app at `http://localhost:8000`

## Usage

1. Open the web interface
2. Upload a satellite image (JPG/PNG)
3. View predicted cyclone intensity

## Project Structure

- `intensitymodel/` - ML prediction logic and Django app
- `rest_api/` - REST API endpoints
- `media/` - Uploaded images
- `model.h5` - Pre-trained ML model
- `Dockerfile` - Container setup

## License

MIT License

## Author

HimanshuxD79
