# File-Handler-TG-Bot

This bot can help you with various file operations including:
* PDF merging, splitting and compressing
* Image resizing, conversion and compressing
* Archive extraction (extract ZIP/RAR/7Z)

Use `/help` to see all available commands.

## To run the bot:

1. Install requirements:
```bash
pip install -r requirements.txt
```

2. Set environment variables:
### Set in the config.py
Fill with your own values,
```python
API_ID = int(os.environ.get("API_ID", ""))
API_HASH = os.environ.get("API_HASH", "")
BOT_TOKEN = os.environ.get("BOT_TOKEN", "")
```
or
### Set via terminal
```bash
export API_ID="your_api_id"
export API_HASH="your_api_hash"
export BOT_TOKEN="your_bot_token"
```

3. Add authorized user IDs in `config.py`

4. Run the bot:
```bash
python main.py
```

___

### Bot Commands

```
mergepdf - Merge multiple PDFs
splitpdf - Split PDF into individual pages
compresspdf - Compress PDF file
resizeimage - Resize images
image2pdf - Convert images to PDF
compressimage - Compress images
unarchive - Extract ZIP/RAR/7Z files
help - Show this help message
status - Show current operation status
done - Tell the bot you're done
cancel - Abort current operation
```

___

To handle such large files efficiently, make sure your server has:
1. Sufficient storage space (at least 3x the maximum total file size)
2. Adequate RAM (recommended 4GB minimum)
3. Good internet connection for handling large file transfers
