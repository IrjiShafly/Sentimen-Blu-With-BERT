Sentiment Analysis of blu by BCA Application Reviews Using IndoBERT

This project is a thesis that focuses on sentiment analysis of reviews for the blu by BCA application, a digital banking platform offering various services such as fund transfers, balance monitoring, and bill payments. With over 10 million downloads and 95,000 reviews on the Google Play Store, this research aims to understand user sentiment to improve the quality of application services.

 Methodology

The sentiment analysis is conducted using the Bidirectional Encoder Representations from Transformers (BERT) method, specifically the IndoBERT pre-trained model. The sentiment of user reviews is classified into three categories:
- Positive
- Neutral
- Negative

 Dataset
- Source: User reviews of the blu by BCA application from the Google Play Store.
- Size: 20,000 reviews in Indonesian, collected via web scraping.
- Data Split: 
  - Training: 70%
  - Validation: 20%
  - Test: 10%

 Preprocessing Steps
1. Case Folding: Converting text to lowercase.
2. Data Cleaning: Removing unwanted characters, links, and symbols.
3. Tokenization: Splitting text into individual tokens.
4. Normalization: Standardizing informal words to their correct forms.

 Evaluation
The model is evaluated using a confusion matrix, achieving:
- Overall Accuracy: 83%
- Positive Sentiment Accuracy: 84%
- Neutral Sentiment Accuracy: 19%
- Negative Sentiment Accuracy: 89%

 Key Results
The research highlights that the model effectively detects positive and negative sentiments but struggles with neutral sentiments due to limited data in this category. 

 Future Improvements
1. Increasing the dataset size for neutral and negative sentiments to balance the data.
2. Using a larger pre-trained model, such as IndoBERTLARGE, for better performance.
3. Experimenting with hyperparameter tuning to optimize the model further.

 Conclusion
This project contributes to understanding user satisfaction with the blu by BCA application and serves as a foundation for developing advanced sentiment analysis models in the future.

 Dependencies
- Python 3.8+
- Transformers Library
- Scikit-learn
- Pandas
- PyTorch

 How to Run
1. Clone the repository:  
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the training script:  
   ```bash
   python train_model.py
   ```
4. Evaluate the model:  
   ```bash
   python evaluate_model.py
   ```

 License
This project is licensed under the MIT License. See the `LICENSE` file for details.
```MIT License

Copyright (c) 2024 Irji Shafly Ridhan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.```
