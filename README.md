# HireGPT

The Resume Ranking App is a Python application built with Streamlit that allows you to rank and shortlist resumes based on their similarity to a given job description. It uses Natural Language Processing (NLP) techniques to extract skills and projects from resumes and then calculates the similarity between the job description and each resume using the Term Frequency-Inverse Document Frequency (TF-IDF) vectorizer and cosine similarity.

## Features

- Upload job title and job description.
- Upload multiple resumes in supported formats (PDF, DOCX, or TXT).
- Rank the resumes based on their similarity score with the job description.
- Shortlist candidates whose similarity score meets the specified threshold.
- Extract contact information (emails and phone numbers) from shortlisted resumes.

## How to Use

1. Install the required dependencies:
   ```bash
   pip install streamlit nltk PyPDF2 textract docx openai langchain
   ```

2. Set your OpenAI API key as an environment variable:
   ```bash
   export OPENAI_API_KEY=your_openai_api_key_here
   ```

3. Run the app using Streamlit:
   ```bash
   streamlit run app.py
   ```

4. Enter the job title, job description, and upload resumes to start the ranking process.

## Dependencies

- [Streamlit](https://www.streamlit.io/)
- [NLTK](https://www.nltk.org/)
- [PyPDF2](https://pythonhosted.org/PyPDF2/)
- [textract](https://textract.readthedocs.io/en/stable/)
- [python-docx](https://python-docx.readthedocs.io/en/latest/)
- [openai](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_generate_text_with_GPT_3.ipynb)
- [langchain](https://pypi.org/project/langchain/)

## Note

- This app uses the OpenAI API to extract skills and projects from resumes. Make sure you have set your OpenAI API key as an environment variable (OPENAI_API_KEY) before running the app.

- The app currently supports resumes in PDF, DOCX, and TXT formats. Make sure to upload the resumes in these formats for accurate processing.

- For security reasons, do not share your OpenAI API key publicly or commit it to version control systems.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as per the license terms.

## Disclaimer

This project is for demonstration purposes only and not intended for production use. The accuracy of resume ranking may vary depending on the quality of the job description and the resumes provided. Always verify and validate the results before making any hiring decisions.

## Author

[Nilesh Ranjan Pal](https://github.com/smallboy713102)
