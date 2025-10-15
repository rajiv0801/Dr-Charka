# Dr. Charaka - AI-Powered Healthcare Platform

Dr. Charaka is a comprehensive AI-powered healthcare platform that combines medical predictions, chat functionality, community support, and medical news updates.

## Features

- **AI Medical Chat**: Interact with an AI-powered medical assistant
- **Disease Prediction Models**:
  - Heart Disease Prediction
  - Diabetes Prediction
  - Liver Disease Prediction
  - Breast Cancer Prediction
- **Medical Community**: Share and discuss medical cases
- **Drug Interaction Checker**: Check potential drug interactions
- **Medical News**: Stay updated with latest medical news
- **User Management**: Complete authentication system with email verification

## Tech Stack

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Database**: SQLite
- **AI/ML**: XGBoost, Random Forest
- **APIs**: Groq API, News API

## Prerequisites

- Python 3.8+
- pip (Python package manager)
- Virtual environment (recommended)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/rajiv0801/Dr-Charka.git
   cd Dr-Charka
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On Unix or MacOS
   source venv/bin/activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the root directory and add your API keys:
   ```env
   GROQ_API_KEY=your_groq_api_key
   NEWS_API_KEY=your_news_api_key
   DJANGO_SECRET_KEY=your_django_secret_key
   DEBUG=True
   ```

5. Run migrations:
   ```bash
   python manage.py migrate
   ```

6. Create a superuser (admin):
   ```bash
   python manage.py createsuperuser
   ```

7. Run the development server:
   ```bash
   python manage.py runserver
   ```

The application will be available at `http://127.0.0.1:8000/`

## Environment Variables

The following environment variables are required:

- `GROQ_API_KEY`: API key for Groq AI services
- `NEWS_API_KEY`: API key for medical news integration
- `DJANGO_SECRET_KEY`: Django secret key
- `DEBUG`: Boolean for debug mode (True/False)

## Project Structure

```
dr-charaka/
├── accounts/         # User authentication and profiles
├── community/        # Medical community features
├── conversation/     # Chat functionality
├── core/            # Core application features
├── drug_interaction/# Drug interaction checker
├── llm/             # AI language model integration
├── medical_news/    # Medical news integration
├── predictor/       # Disease prediction models
├── static/          # Static files (CSS, JS)
├── templates/       # HTML templates
└── mediai/          # Project settings
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to all contributors who have helped shape Dr. Charaka
- Medical datasets used for training the prediction models
- Open source community for various tools and libraries used

## Support

For support, contact me through this [Gmail](mailto:rajivrajput2005@gmail.com) or open an issue in the repository.
