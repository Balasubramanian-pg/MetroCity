### **2. Unstructured & Semi-Structured Data**

This category captures customer interactions, sentiment, and behavior from various digital touchpoints, providing context beyond simple transactions.

| Data Asset | Source File | Description | Key Attributes | Role in the Project |
| :--- | :--- | :--- | :--- | :--- |
| **Product Reviews** | `product_reviews.json` | Customer-submitted reviews and star ratings for specific products purchased. | `CustomerID`, `ProductID`, `Rating` (1-5), `ReviewText`, `Timestamp` | Used to calculate the average product rating, identify top- and bottom-rated products, and understand customer satisfaction at a product level. |
| **Social Media Mentions** | `social_media.json` | Aggregated brand mentions and associated sentiment from various social media platforms. | `Platform` (e.g., Twitter, Facebook), `Content`, `Sentiment` (Positive, Neutral, Negative) | Provides insight into public brand perception and allows for tracking overall customer sentiment trends across different online communities. |
| **Weblog Engagement** | `web_blogs.json` | Server logs capturing user actions and engagement on the company's website or e-commerce platform. | `UserID`, `Action` (View, Click, AddToCart, Purchase), `Page` (e.g., Homepage, Product Page) | Helps analyze the customer journey on the website, understand conversion funnels (from view to purchase), and measure user engagement. |
