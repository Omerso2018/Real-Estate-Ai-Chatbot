# Real-Estate-Ai-Chatbot
# 🏠 Real Estate AI Chatbot Widget

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

---

## 📦 Installation

1. **Download** or **clone** this repository:
   ```bash
   git clone https://github.com/yourusername/real-estate-ai-chatbot.gi
2. Add the chatbot HTML file to your real estate website:

Place the wp-real-estate-agent.html in your project or theme folder.
 
Include it in your site via an iframe or directly embed the code in your WordPress theme.

3. Configure your chatbot in the script section:

Replace YOUR_OPENROUTER_API_KEY_HERE with your OpenRouter API key.

Replace https://yourdomain.com/wp-json/wp/v2/property with your WordPress property endpoint URL.  

------------
🔌 WordPress REST API Setup

Ensure your WordPress site has:

Property Custom Post Type (e.g., property)

REST API enabled

Custom meta fields for price, location, bedrooms, bathrooms, area, and property type.

Example endpoint:
 ```
https://yourdomain.com/wp-json/wp/v2/property
 ```
You can filter results by adding query params such as:
 ```
?search=London&max_price=500000&min_bedrooms=3
 ```
-----------

#🚀 Usage

Click the floating chat icon to open the chatbot.

Ask questions like:

"Find me an apartment in New York under $800,000"

"Show me houses in Dubai with 4 bedrooms"

The chatbot will:

Detect your intent and extract filters.

Fetch matching properties from your WordPress site.

Display them as interactive cards in the chat.

##🛡️ Rate Limiting & Caching

AI API calls are limited to 8 per minute by default.

Property API calls are limited to 5 per minute with a 5-minute cache.

These values can be adjusted in the configuration.

##📄 License

This project is licensed under the MIT License – see the LICENSE file for details.
