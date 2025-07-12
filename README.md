  <h1>🧠 Sentiment Analysis on Tweets using LSTM</h1>

  <p>This project performs sentiment analysis on tweets using a Long Short-Term Memory (LSTM) deep learning model. The goal is to classify the sentiment of each tweet as <strong>positive</strong>, <strong>neutral</strong>, or <strong>negative</strong> using the <a href="https://www.kaggle.com/datasets/kazanova/sentiment140" target="_blank">Sentiment140 dataset</a>.</p>

  <h2>📂 Dataset</h2>
  <ul>
    <li><strong>Source:</strong> <a href="https://www.kaggle.com/datasets/kazanova/sentiment140" target="_blank">Sentiment140 Dataset on Kaggle</a></li>
    <li><strong>Size:</strong> 1.6 million labeled tweets</li>
    <li><strong>Labels:</strong>
      <ul>
        <li>0: Negative</li>
        <li>2: Neutral</li>
        <li>4: Positive</li>
      </ul>
    </li>
  </ul>

  <h2>🛠 Features</h2>
  <ul>
    <li>Data cleaning (removing links, special characters, and lowercasing)</li>
    <li>Tokenization and sequence padding</li>
    <li>Text vectorization with TensorFlow's Tokenizer</li>
    <li>Sentiment classification using an LSTM model</li>
    <li>Model evaluation using accuracy, classification report, and confusion matrix</li>
    <li>Live predictions on custom user input</li>
  </ul>

  <h2>🧪 Model Architecture</h2>
  <pre><code>Embedding → LSTM → Dropout → Dense (Softmax)</code></pre>
  <ul>
    <li>Embedding Layer with 10,000 vocabulary size</li>
    <li>LSTM with 64 hidden units</li>
    <li>Dropout for regularization</li>
    <li>Output layer with 3 softmax-activated units for multi-class classification</li>
  </ul>

  <h2>📊 Results</h2>
  <ul>
    <li><strong>Validation Accuracy:</strong> ~82%</li>
    <li><strong>Test Accuracy:</strong> Varies based on split</li>
    <li>Model performs well on positive/negative, slightly under on neutral</li>
  </ul>

  <h2>🚀 How to Run</h2>
  <pre><code>git clone https://github.com/wasayfaizan/sentiment140-lstm.git
cd sentiment140-lstm

pip install -r requirements.txt

# Run the notebook or script to train the model
</code></pre>

  <h2>🧠 Example: Custom Predictions</h2>
  <pre><code>predict_sentiment("I really love this product!")
# Output: Positive (99%)

predict_sentiment("This is the worst app I've used.")
# Output: Negative (97%)

predict_sentiment("It’s okay, not bad but not amazing.")
# Output: Neutral or Negative depending on tuning
</code></pre>

  <h2>📁 Folder Structure</h2>
  <pre><code>sentiment140-lstm/
├── sentiment140.csv
├── lstm_model.ipynb
├── lstm_confusion_matrix.png
├── requirements.txt
└── README.md
</code></pre>



</body>
</html>
