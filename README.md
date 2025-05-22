### Text-to-Speech-pidgin Text Dataset.
#### Project Overview
This project preprocesses a pidgin text dataset is suitable for natural language processing (NLP) tasks involving Pidgin English.Texts are sourced from biblical scripture in Nigerian Pidgin, which maintains cultural and linguistic relevance.100 entries — small enough for quick prototyping, yet sufficient for demonstrating basic NLP techniques, Nigerian Pidgin and it is open use or publication.
#### Objective
To clean and analyze pidgin text data for potential use in language modeling or chatbot training.
#### Data Source
Name: www.Hugging face.com
Titled "Bible dataset in Pidgin"
Data Format:xlsx (Excel spreadsheet)
Column Name: pidginstring
No of Rows: 100 and No of Columns: 1
#### Data Cleaning and Processing
Remove special characters and formatting issues (e.g., strange encoding like “â€”” or “â€”).
Dropping Missing Rows vs Filling Missing Values: No missing values.
Removing Duplicates or Keeping Them: No duplicates found. 
Convert to lowercase.
Word Count TransformationWhy: Useful for text length analysis.
### Final Data Summary (After cleaning)
Total sentences: 100
Average words per sentence: 22.84
Total words: 2284,[('di', 91), ('dey', 88), ('for', 74), ('and', 72), ('go', 72), ('wey', 68), ('dem', 48), ('una', 43), ('god', 36), ('make', 36)] 
