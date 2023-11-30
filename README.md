# Vector Space Model for Medical Records Search Engine

## **Information Retrieval Final Project**

Peter Johan Arkadhira Setiabudi - 21/475025/PA/20510

Putu Arva Raysendriya Ersuputra - 21/472606/PA/20312

Henzel Theodore Putra - 21/475040/PA/20516

Muhammad Alfi Ramadhan - 21/472839/PA/20345

## Features

- **Data Preprocessing**: The medical records dataset is preprocessed by tokenizing, lowercasing, and combining relevant fields.

- **TF-IDF Vectorization**: The combined text is transformed into a TF-IDF matrix using the scikit-learn library.

- **Query Processing**: Queries are preprocessed, and the cosine similarity between the query and documents is calculated to retrieve relevant results.

- **Search Engine Queries**: Four example queries are provided, each searching for different information types such as doctors for a patient, patients for a doctor, medicines for a patient, and medicines prescribed by a doctor.

- **Evaluation Metrics**: Precision and recall are calculated for each query to assess the search engine's performance.

## Getting Started

1. Install the required dependencies by running:

   ```bash
   !pip install nltk
   ```

2. Download the NLTK punkt tokenizer:

   ```python
   import nltk
   nltk.download('punkt')
   ```

3. Load the medical records dataset by providing the path to your CSV file:

   ```python
   df = pd.read_csv('/path/to/your/medical/records.csv')
   ```

4. Run the search engine queries and evaluate the results:

   ```python
   # Example Queries
   query_1 = "find doctor for patient noah hidayat"
   # ... (provide queries for other use cases)

   # Customize keywords for relevance
   relevant_keywords_1 = ['noah', 'hidayat']
   # ... (provide relevant keywords for other use cases)

   # Run the search
   query_type_1, results_1, count_1, relevant_count_1 = search(query_1, relevant_keywords=relevant_keywords_1)
   # ... (repeat for other queries)

   # Calculate precision and recall
   precision1 = relevant_count_1 / count_1
   recall1 = relevant_count_1 / ground_truth1
   # ... (repeat for other queries)

   # Print results and evaluation metrics
   ```

## Results and Evaluation

The search engine's performance is evaluated using precision and recall for each query. The results and metrics for the example queries are displayed in the console output.

### Query 1: Find doctor for patient Noah Hidayat

- Precision: {precision1}
- Recall: {recall1}

### Query 2: Find patient for doctor Anita

- Precision: {precision2}
- Recall: {recall2}

### Query 3: Find medicine for patient Guntur

- Precision: {precision3}
- Recall: {recall3}

### Query 4: Find medicine by doctor Yudhisindo

- Precision: {precision4}
- Recall: {recall4}

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Special thanks to the NLTK and scikit-learn communities for their valuable contributions.

Feel free to adapt this README to better fit your project and provide more details if needed.
