# AI-Powered Data Science Report Generator

A comprehensive web application that automates data science workflows by accepting datasets, performing analysis, training machine learning models, and generating professional reports with AI-powered insights.

## 🚀 Features

### Frontend (Next.js)
- **Drag & Drop File Upload**: Easy dataset upload with support for CSV and Excel files
- **Interactive Configuration**: Configure analysis type, target variables, and model selection
- **Real-time Progress Tracking**: Visual progress indicators during analysis
- **Comprehensive Reports**: Rich visualizations and AI-generated insights
- **Export Functionality**: Download professional PDF reports

### Backend (Python FastAPI)
- **Automated Data Cleaning**: Handle missing values and outliers
- **Exploratory Data Analysis**: Statistical summaries and visualizations
- **Machine Learning Pipeline**: Multiple model training and evaluation
- **AI-Powered Insights**: GPT-generated analysis and recommendations
- **RESTful API**: Clean API endpoints for frontend integration

## 🛠️ Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first styling
- **shadcn/ui** - Modern UI components
- **Recharts** - Data visualization library
- **Radix UI** - Accessible component primitives

### Backend
- **FastAPI** - Modern Python web framework
- **Pandas & NumPy** - Data manipulation and analysis
- **Scikit-learn** - Machine learning algorithms
- **Matplotlib & Seaborn** - Data visualization
- **OpenAI API** - AI-powered insights generation

## 📊 Supported Analysis Types

1. **Exploratory Data Analysis (EDA)**
   - Statistical summaries
   - Correlation analysis
   - Distribution plots
   - Missing value analysis

2. **Classification**
   - Random Forest Classifier
   - Logistic Regression
   - Support Vector Machine
   - XGBoost
   - Neural Networks

3. **Regression**
   - Linear Regression
   - Random Forest Regressor
   - XGBoost Regressor
   - Ridge & Lasso Regression

4. **Clustering**
   - K-Means
   - DBSCAN
   - Hierarchical Clustering
   - Gaussian Mixture Models

5. **Time Series Forecasting**
   - ARIMA
   - Prophet
   - LSTM
   - Exponential Smoothing

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm
- Python 3.8+
- OpenAI API key (for AI insights)

### Frontend Setup
\`\`\`bash
# Install dependencies
npm install

# Start development server
npm run dev
\`\`\`

### Backend Setup
\`\`\`bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install fastapi uvicorn pandas numpy scikit-learn matplotlib seaborn openai python-multipart

# Start API server
python scripts/backend-api-example.py
\`\`\`

### Environment Variables
Create a `.env.local` file in the root directory:
\`\`\`
OPENAI_API_KEY=your_openai_api_key_here
NEXT_PUBLIC_API_URL=http://localhost:8000
\`\`\`

## 📁 Project Structure

\`\`\`
data-science-generator/
├── app/                          # Next.js app directory
│   ├── page.tsx                 # Main application page
│   ├── layout.tsx               # Root layout
│   └── globals.css              # Global styles
├── components/                   # React components
│   ├── ui/                      # shadcn/ui components
│   ├── data-upload.tsx          # File upload component
│   ├── analysis-config.tsx      # Configuration form
│   ├── progress-tracker.tsx     # Progress visualization
│   └── report-viewer.tsx        # Report display
├── scripts/                     # Backend scripts
│   └── backend-api-example.py   # FastAPI backend
├── lib/                         # Utility functions
└── public/                      # Static assets
\`\`\`

## 🔄 Workflow

1. **Upload Dataset**: Drag and drop CSV/Excel files
2. **Configure Analysis**: Select analysis type, target variables, and models
3. **AI Processing**: Automated data cleaning, EDA, and model training
4. **View Results**: Interactive reports with visualizations and insights
5. **Export Report**: Download comprehensive PDF reports

## 📈 Example Use Cases

- **Sales Forecasting**: Predict future sales based on historical data
- **Customer Segmentation**: Cluster customers for targeted marketing
- **Performance Analysis**: Analyze employee performance factors
- **Risk Assessment**: Classify loan default probability
- **Quality Control**: Predict product defects from manufacturing data

## 🤖 AI-Powered Features

- **Automated Insights**: GPT-generated analysis summaries
- **Smart Recommendations**: Data-driven business suggestions
- **Natural Language Reports**: Human-readable explanations
- **Feature Importance**: AI-explained variable significance

## 🔧 Customization

The application is designed to be highly customizable:

- **Add New Models**: Extend the model library in the backend
- **Custom Visualizations**: Add new chart types using Recharts
- **Report Templates**: Modify report layouts and styling
- **API Integration**: Connect to external data sources

## 📝 API Endpoints

- `POST /api/upload` - Upload and analyze dataset
- `POST /api/analyze` - Perform configured analysis
- `GET /api/export-report` - Export analysis report

## 🚀 Deployment

### Frontend (Vercel)
\`\`\`bash
npm run build
# Deploy to Vercel
\`\`\`

### Backend (Docker)
\`\`\`dockerfile
FROM python:3.9
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
\`\`\`

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- OpenAI for GPT API
- Vercel for hosting platform
- shadcn for UI components
- The open-source data science community
