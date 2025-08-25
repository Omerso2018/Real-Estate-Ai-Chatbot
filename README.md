# Real Estate AI Agent Chatbot 🏠
# WordPress Real-Estate Chatbot Widget

An interactive, AI-powered real estate chatbot widget designed to act as a **virtual property agent** for real estate websites.  
It integrates with the **[OpenRouter API](https://openrouter.ai/)** for natural conversation and property search intent detection, and fetches **real-time property listings** from a **WordPress REST API** endpoint.  

![Real Estate Chatbot Preview](https://via.placeholder.com/800x400?text=Real+Estate+AI+Chatbot+Preview)

---

## ✨ Features

- **AI Conversation** – Powered by OpenRouter API for natural, friendly, and professional responses.
- **Property Search** – Extracts location, price range, property type, and more from user queries.
- **WordPress Integration** – Retrieves and filters property data directly from your WP site via REST API.
- **Smart Filtering** – AI + regex-based extraction for robust query interpretation.
- **Property Cards Display** – Shows property images, details, and “View Details” links in chat.
- **Responsive UI** – Works on desktop and mobile with modern, animated UI.
- **Rate Limiting & Caching** – Prevents API overuse and optimizes data fetching.
- **Customizable Theme** – Easily adjust colors, avatars, and chatbot name.

## 🚀 Quick Start

### 1. Download the Files
```bash
git clone https://github.com/yourusername/real-estate-chatbot.git
cd real-estate-chatbot
 ```
### 2. Configure API Keys
Open real-estate-chatbot.html and update the configuration:
```
const config = {
    // Replace with your OpenRouter API key
    apiKey: 'YOUR_OPENROUTER_API_KEY_HERE',
    
    // Replace with your WordPress API URL
    wpApiUrl: 'https://yoursite.com/wp-json/wp/v2/property',
    
    // Optional: WordPress API authentication
    wpApiKey: 'YOUR_WP_API_KEY',
    
    // Customize bot name and theme
    botName: 'Your Real Estate AI',
    primaryColor: '#dc2626',
    secondaryColor: '#ef4444'
};
 ```

------------------------------------------

## 📝 How It Works
#### 1. Information Gathering
The chatbot follows a structured conversation flow:
- Purpose (Buy/Rent)
- Location preferences
- Budget range
- Number of bedrooms
- Property type
- Additional preferences
### 2. AI Processing
- Extracts information from natural language
- Maintains conversation context
- Generates relevant responses
- Handles complex user queries
### 3. Property Search
- Queries WordPress API with user preferences
- Applies intelligent filtering
- Caches results for performance
- Displays properties in beautiful cards
### 4. User Interaction
- Click property cards to view details
- Use quick action buttons
- Natural conversation flow
- Mobile-responsive interface

  
## 🛡️ API Call Mechanism 
### this chatbot with work by 4 API call consist of ( 3 AI modele work as agents + one WordPress REST API) that connected in a single pipeline:

- Agent 1 (Extractor) → turns the user’s message into structured filters (fast, free model)

- WordPress REST API → fetches properties using those filters (server-side filtering where possible + client-side fallback)

- Agent 2 (Formatter) → crafts a friendly, human-readable reply using the properties JSON

- Agent 3 (complex Response) → this to take and hanlde user conplex responses
  

------------------------------------------------------------------------  

## 📄 License
This project is open source and available under the MIT License.

## 🤝 Contributing
Contributions are welcome! Please:

- Fork the repository
- Create a feature branch
- Make your changes
- Test thoroughly
- Submit a pull request
### Made with ❤️ for the real estate industry

### ⭐ If you find this useful, please give it a star on GitHub!
