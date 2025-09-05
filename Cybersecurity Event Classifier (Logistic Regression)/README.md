## Project 1: Cybersecurity Event Classifier (Logistic Regression)

This project uses **Logistic Regression** to classify cybersecurity events, including normal traffic, phishing attempts, DoS attacks, and malware activities. It demonstrates how machine learning can analyze numeric features from network or system data to detect security threats.

**How it works (detailed):**

1. **Data Preparation:**  
   - The dataset contains numeric features such as `packet_size`, `failed_logins`, `suspicious_port`, and `connection_duration`.  
   - The categorical target (`event_type`) is converted into numeric labels using **Label Encoding** so the model can process it.

2. **Feature Scaling:**  
   - All features are standardized using **StandardScaler** so that they have a mean of 0 and a standard deviation of 1.  
   - Scaling ensures that features with larger numeric ranges do not dominate the model’s learning process.

3. **Model Training:**  
   - **Logistic Regression** is trained on the scaled data.  
   - Each feature is assigned a **coefficient (weight)**, indicating how strongly it influences the prediction of each class.  
   - The model calculates a weighted sum of features for each input, then applies a **sigmoid function** to convert this sum into a probability between 0 and 1.

4. **Multiclass Prediction:**  
   - Since there are multiple event types, the model uses a **softmax-like approach** to compute probabilities for all classes.  
   - The predicted class is the one with the highest probability.

5. **Evaluation:**  
   - The model is tested on a separate portion of the dataset to measure **accuracy**, indicating how well it predicts unseen events.

6. **User Input Testing:**  
   - Users can input a new event’s feature values interactively.  
   - The model outputs both the predicted event type and the probability for each class, allowing interpretation of confidence.

7. **Visualization:**  
   - A scatter plot can show relationships between features, colored by event type.  
   - A bar chart of feature coefficients highlights which features most influence the model’s decisions.

This detailed pipeline demonstrates how numeric network or system features can be transformed, analyzed, and used for **automated cybersecurity threat classification**.
