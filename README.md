# Tesouro Direto Monitor

## 🔹 Description

**Tesouro Direto Monitor** is a Python script designed to automate data collection from Tesouro Direto, process the information, and send real-time updates via Telegram. It uses Selenium for web data extraction and organizes bonds based on the best returns.

## 🔹 Features

- Automatic data collection from Tesouro Direto.
- Processing and classification of government bonds (IPCA+, Fixed Rate, etc.).
- Custom message formatting for Telegram.
- Automatic updates sent via a Telegram bot.

## 🔹 Technologies Used

- **Python 3.13.1**
- **Selenium** for browser automation.
- **pylegram** for Telegram integration.
- **JSON** for data handling.

## 🔹 Installation

```bash
# Clone the repository
git clone https://github.com/your-username/your-repository.git
cd your-repository

# Install dependencies
pip install -r requirements.txt

# Configure the Chrome WebDriver to match your browser version
```

## 🔹 Configuration

- **Telegram Token:** Update the bot token and `chat_id` in the `MessageSender` file with your credentials.
- **WebDriver:** Adjust Selenium settings if necessary (e.g., headless mode).

## 🔹 How to Use

```bash
# Run the main script
python main.py
```

The script will:
- Fetch updated Tesouro Direto data.
- Process bonds to display the best returns.
- Send a formatted message to Telegram.

## 🔹 Project Structure

```plaintext
.
├── main.py              # Main script
├── requirements.txt     # Project dependencies
├── README.md            # Documentation
└── src/
    ├── chrome_config.py   # WebDriver configuration
    ├── data_fetcher.py    # Data collection from Tesouro Direto
    ├── data_processor.py  # Data processing
    ├── message_formatter.py  # Message formatting
    └── message_sender.py     # Sending messages via Telegram
```

## 🔹 Output Example

```plaintext
🤖 *Monitoring #TesouroDireto*

*IPCA+*
• 2029  5.75%  R$1010.00

*Fixed Rate*
• 2026  10.25%  R$950.00

#investments #fixedincome #IPCA
```
