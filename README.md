# Vector Space Model for Medical Records Search Engine

**Information Retrieval Final Project**

Peter Johan Arkadhira Setiabudi - 21/475025/PA/20510

Putu Arva Raysendriya Ersuputra - 21/472606/PA/20312

Henzel Theodore Putra - 21/475040/PA/20516

Muhammad Alfi Ramadhan - 21/472839/PA/20345



**Overview**

This repository contains Python code that implements a vector space model for a search engine tailored for medical records. The vector space model is used to efficiently search and retrieve relevant information from a dataset containing doctor-patient-medicine combinations.



**Features**

Data Preprocessing: The medical records dataset is preprocessed by tokenizing, lowercasing, and combining relevant fields.

TF-IDF Vectorization: The combined text is transformed into a TF-IDF matrix using the scikit-learn library.

Query Processing: Queries are preprocessed, and the cosine similarity between the query and documents is calculated to retrieve relevant results.

Search Engine Queries: Four example queries are provided, each searching for different information types such as doctors for a patient, patients for a doctor, medicines for a patient, and medicines prescribed by a doctor.

Evaluation Metrics: Precision and recall are calculated for each query to assess the search engine's performance.


