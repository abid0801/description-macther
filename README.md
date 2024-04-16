## Description Similarity Calculator

This Python script calculates the similarity between two descriptions using the TF-IDF vectorization method and cosine similarity.

### Dependencies

- Python 3.x
- scikit-learn (`sklearn`)

### Installation

1. Ensure you have Python installed. If not, download and install it from [here](https://www.python.org/downloads/).
2. Install scikit-learn package using pip:

    ```
    pip install scikit-learn
    ```

### Usage

1. Import the necessary functions from the script:

    ```python
    from sklearn.feature_extraction.text import TfidfVectorizer
    from sklearn.metrics.pairwise import cosine_similarity
    ```

2. Define or import the following functions:

    - `preprocess_text(text)`: Preprocesses the input text by converting it to lowercase and removing non-alphanumeric characters.
    - `calculate_similarity(description1, description2, threshold)`: Calculates the similarity between two descriptions. The optional `threshold` parameter specifies the minimum similarity score required for the descriptions to be considered similar.
    - `compare_descriptions(description1, description2)`: Compares two descriptions and returns the similarity score.

3. Provide descriptions to compare:

    ```python
    description1 = "Loaded with BBQ-infused beef pepperoni, savory imported chicken sausage, gooey imported mozzarella, fresh capsicum, zesty green chili, tangy black olives, all smothered in a rich BBQ-soaked marinara sauce."
    description2 = "Topped with Beef Pepperoni (BBQ), Imported Chicken Sausage (BBQ), Imported Mozzarella, Capsicum, Green Chilli, Black Olive, BBQ Soaked Marinara Sauce."
    ```

4. Call the `compare_descriptions` function with the two descriptions:

    ```python
    similarity_score = compare_descriptions(description1, description2)
    ```

5. The `similarity_score` will indicate the similarity between the descriptions. If the similarity score is above a certain threshold (default is 0.7), the descriptions are considered similar.

### Example

```python
similarity_score = compare_descriptions(description1, description2)
print(similarity_score)
```

### Note

- Ensure that descriptions are provided as strings.
- Adjust the threshold parameter according to the desired similarity threshold.

