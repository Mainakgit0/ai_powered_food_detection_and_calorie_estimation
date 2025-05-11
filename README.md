
# 🍏 Smart Food Analyzer

![App Banner](https://via.placeholder.com/1200x400.png?text=Smart+Food+Analyzer)

An AI-powered application that analyzes food images to provide detailed nutritional information, visual comparisons, and dietary recommendations using Google's Gemini AI.

## ✨ Features

- **📸 Image Analysis**: Upload food photos for instant nutritional analysis
- **📊 Nutrition Dashboard**: View calories, macros, and vitamin content
- **📈 Data Visualizations**: 
  - Macronutrient comparison charts
  - Calorie comparison graphs
  - Interactive pie charts
- **💬 AI Nutritionist Chat**: Get personalized dietary advice
- **📥 Report Generation**: Download detailed nutrition reports
- **🌙 Dark Mode**: Automatic theme switching

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/smart-food-analyzer.git
   cd smart-food-analyzer
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up API keys**:
   - Get your Gemini API keys from [Google AI Studio](https://aistudio.google.com/)
   - Update the keys in `food_analyzer.py`:
     ```python
     genai.configure(api_key="YOUR_MAIN_GEMINI_API_KEY")
     GEMINI_CHAT_API_KEY = "YOUR_CHAT_API_KEY"
     ```

## 🚀 Usage

```bash
streamlit run food_analyzer.py
```

**App Workflow**:
1. Upload a food image
2. Specify portion size (weight in grams or servings)
3. View comprehensive nutritional analysis
4. Explore interactive visualizations
5. Chat with the AI nutritionist
6. Download full reports

## 📂 File Structure

```
smart-food-analyzer/
├── food_analyzer.py       # Main application code
├── requirements.txt       # Python dependencies
├── README.md              # This documentation
└── .gitignore             # Standard Python gitignore
```

## 🔧 Requirements

```text
streamlit==1.32.0
google-generativeai==0.3.2
Pillow==10.1.0
pandas==2.1.4
matplotlib==3.8.2
seaborn==0.13.0
numpy==1.26.2
```

## 🎨 Customization

### Food Database
Edit the `FOOD_DATABASE` dictionary to add/remove foods:
```python
FOOD_DATABASE = {
    "Food Name": {
        "calories": X,
        "protein": X,
        "carbs": X,
        "fats": X
    }
}
```

### Daily Values
Modify these constants for personalized targets:
```python
DAILY_CALORIES = 2000
DAILY_MACROS = {"protein": 50, "carbs": 275, "fats": 70}
```

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## ⚠️ Troubleshooting

| Issue | Solution |
|-------|----------|
| API Errors | Verify Gemini API keys and quota |
| Image Analysis Fails | Use clear, well-lit food photos |
| Dependency Issues | Create fresh virtual environment |

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgments

- Google Gemini API
- Streamlit team
- Pandas/Matplotlib/Seaborn communities
```

And here's the `requirements.txt` content:

```text
streamlit==1.32.0
google-generativeai==0.3.2
Pillow==10.1.0
pandas==2.1.4
matplotlib==3.8.2
seaborn==0.13.0
numpy==1.26.2
```

To use these:

1. Create a new repository on GitHub
2. Add these two files:
   - `README.md` (the first content above)
   - `requirements.txt` (the second content above)
3. Add your `food_analyzer.py` with the code you shared
4. Include a `.gitignore` file for Python

The README includes:
- Eye-catching emojis and headers
- Clear installation/usage instructions
- Visual structure with code blocks
- Troubleshooting table
- Contribution guidelines
- License information

