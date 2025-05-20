# Text-to-Speech-pidgin Text Dataset (Build foundational knowledge of how TTS works and the peculiarities of African languages in TTS training)
Data Source:www.Hugging face.com:Titled "Bible dataset in Pidgin",Data Format:xlsx (Excel spreadsheet),Column Name: pidginstring,No of Rows: 100 and No of Columns: 1
### Reason for Dataset Choice
This dataset is suitable for natural language processing (NLP) tasks involving Pidgin English.Texts are sourced from biblical scripture in Nigerian Pidgin, which maintains cultural and linguistic relevance.
100 entries — small enough for quick prototyping, yet sufficient for demonstrating basic NLP techniques, Nigerian Pidgin and it is open use or publication.
### Basic Statistics (Before Cleaning)
Rows: 100, Columns: 1, Missing Values: 0, Duplicate Rows: 0 and Unique Sentences: 100.
### Data Cleaning and Processing
Convert to lowercase: Why?Text data is case-sensitive by default. Converting all characters to lowercase ensures consistency and avoids treating words like "God" and "god" as different entries. Use case:Important for NLP tasks like tokenization, frequency analysis, and text classification.
Remove punctuation: Why? Punctuation marks (e.g., commas, periods, question marks) often do not contribute to the meaning in basic NLP tasks like sentiment analysis or topic modeling.Use case: Reduces noise in the data, especially for word-level analysis.
Remove special characters and formatting issues (e.g., strange encoding like “â€”” or “â€”):Why? These are artifacts from encoding issues (often due to mismatched character encodings like UTF-8 vs ANSI). Use case: Cleaning them ensures readability and avoids corrupt or meaningless tokens in the data.
Word Count TransformationWhy: Useful for text length analysis, summarization, or filtering very short or long texts. Use case: Can be used for: Building histograms of text length, Pruning outliers, Normalizing text and input sizes.
Dropping Missing Rows vs Filling Missing Values: No missing values. If there were missing entries: Drop if the data is textual and the content is completely empty. Fill only if context allows for safe imputation (e.g., using a placeholder like "unknown"), which is not ideal for scripture.
Removing Duplicates or Keeping Them: No duplicates found. General Rule: Remove duplicates if repeated entries are likely due to copying errors or redundant data. Keep duplicates if repetition reflects real-world meaning (e.g., poetic repetition in scriptures).
### Final Data Summary (After cleaning)
Total sentences: 100, Average words per sentence: 22.84, Total words: 2284,[('di', 91), ('dey', 88), ('for', 74), ('and', 72), ('go', 72), ('wey', 68), ('dem', 48), ('una', 43), ('god', 36), ('make', 36)]
### Challenges and Lessons Learned
The challenge was more about downloading the dataset from the hugging face and File Upload Issues on Google Colab. Observation saw a lot of datasets that were clean already and required minimal pre-processing. 
