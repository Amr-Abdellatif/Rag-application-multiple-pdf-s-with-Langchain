# Rag with multiple PDf's


https://github.com/user-attachments/assets/db5654ee-1e50-4945-b4bb-b708a7a72c15



# getting started and installation
1. Install Ollama from here `https://ollama.com/download`
2. open cmd and write the following command to install llama3:8b from ollama server `ollama run llama3:8b`
3. now you have the LLM isntalled on your machine , just clone the repo 
4. make a venv using `pythoon -m venv venv` this will create a venv called venv
5. open vscode and activate your venv by writing the following in cmd `.\venv\Scripts\activate`
6. install reqirements.txt
7. insert your pdf files into `data` directory
8. run the populate_database.py script to build you embedding database
9. run the query_data.py script to run the app soething like the following `python .\query_data.py "who are the contributors from micknsey and company?"` -> excution criteria is like `.\query_data.py  "question" `
10. there's a test_rag.py script that needs pytest to run if you want to test the application `pytest ./test_rag.py`