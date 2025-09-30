# QA_RAG
這是一個透過RAG製作的QA機器人

1. 使用前請先確認使否有啟動 ollama 並且具備 gpt-oss:20b 這個模型<br>
   (若無請先至 https://ollama.com/ 下載 並且在powershell執行 `ollama pull gpt-oss:20b` )<br>
   下載完後可以執行 `ollama ls` 確認是否有下載成功
2. 在powershell移動到 (cd <資料夾路徑>) 該資料夾的位置, 或是透過 vscode 開啟
3. 接著需要安裝套件，可以直接使用<br>
   `pip install gradio numpy faiss-cpu torch sentence-transformers langchain-core langchain-ollamapython-docx openpyxl python-pptx pillow pdfplumberpaddleocr paddlepaddlelangchain`
5. 再來把回答的 sourcedata(例如操作手冊、導覽手冊等) 放到 data 這個資料夾中
6. 在 terminal 輸入 `python app.py` 即可執行
7. 執行後會出現一個 `Running on local URL: http://127.0.0.1:你的端口`<br>
   點開之後就可以打開使用者介面開始使用

如果有需要更改 sourcedata請先在 terminal 按 crtl + C 中斷執行,並且替換資料再重新啟動即可

成功啟動後的介面如下:
<img width="1888" height="868" alt="image" src="https://github.com/user-attachments/assets/73690b18-fbc2-457e-b3c4-4e1cc31af34b" />
