# Climbing Schedule

## Setup

Make sure you have python3.8 and virtualenv installed. Then run:
```
virutalenv venv
source venv/bin/activate
pip install -r requirements.txt
```

To launch jupyterlab run:
```
jupyter lab
```

## Download the data
Create an export of the Whatsapp chat (zip file) and download it to the `data/` directory. Make sure the file is called `WhatsApp Chat - Entrenos M-J 13-15.zip` or update the filename on the `scripts/parse_chat.ipynb` notebook.

## Extracting training sessions from the chat data
First run the `scripts/parse_chat.ipynb` notebook. This will create a chat.parquet file in `data/` with the chat messages and some metadata. Next run the `script/query.ipynb` notebook that will query for training session messages and export them to a csv in `out/`
