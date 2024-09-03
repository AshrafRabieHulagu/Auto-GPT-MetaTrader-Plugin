Auto-GPT MetaTrader Plugin 📈

The AutoGPT MetaTrader Plugin is a software tool that enables traders to connect their MetaTrader 4 or 5 trading account to Auto-GPT.

Try MetaTrader GPT on ChatGPT

GitHub Repo stars

💖 Help Support Auto-GPT Plugin's Development 💖

If you can spare a coffee, you can help to cover the costs of developing Auto-GPT Plugins and help to push the boundaries of fully autonomous AI! Your support is greatly appreciated. Development of this free, open-source project is made possible by all the contributors and sponsors. If you'd like to sponsor this project and have your avatar or company logo appear below click here.

Crypto Donations: 0x2457e8746EFa5894b70aE06a1b391474bc928B05

💡 Key Features:

💰 Place Trades
ℹ️ Account Information
⛔️ Close Trade
❌ Close All Trades
🕯 Candlestick Data
📈 Stock of The Day
📂 Red Folder News
％ Community Sentiment (In-Progress)
📝 Modify Trades (In-Progress)

🔧 Installation

Follow these steps to configure the Auto-GPT MetaTrader Plugin:

1. Clone the Auto-GPT-MetaTrader-Plugin repository

Clone this repository and navigate to the Auto-GPT-MetaTrader-Plugin folder in your terminal:

git clone https://github.com/AshrafRabieHulagu/Auto-GPT-MetaTrader-Plugin.git

2. Install required dependencies

Execute the following command to install the necessary dependencies:

pip install -r requirements.txt

3. Package the plugin as a Zip file

Compress the Auto-GPT-MetaTrader-Plugin folder or download the repository as a zip file.

5. Install Auto-GPT

If you haven't already, clone the Auto-GPT repository, follow its installation instructions, and navigate to the Auto-GPT folder.

You might have to run this in the Auto-GPT file if you get an error saying "No Module Found".

pip install ta myfxbook

5. Copy the Zip file into the Auto-GPT Plugin folder

Transfer the zip file from step 3 into the plugins subfolder within the Auto-GPT repo.

7. Locate the .env.template file

Find the file named .env.template in the main /Auto-GPT folder.

9. Create and rename a copy of the file

Duplicate the .env.template file and rename the copy to .env inside the /Auto-GPT folder.

11. Edit the .env file

Open the .env file in a text editor. Note: Files starting with a dot might be hidden by your operating system.

13. Add MetaTrader configuration settings

Append the following configuration settings to the end of the file:

################################################################################
### METATRADER
################################################################################
META_API_ACCOUNT_ID=
META_API_TOKEN=
META_API_REGION=
LUNAR_CRUSH_API_KEY=
MY_FX_BOOK_USERNAME=
MY_FX_BOOK_PASSWORD=
FCS_API_KEY=
Create a MetaAPI account and connect to your broker.
MT5 accounts will need to have a paid account to access candlestick data.
Create a MyFxBook account and connect to your trading accounts.
Create a FCS API account. (500 calls/mo for free)
Set META_API_ACCOUNT_ID to your MetaAPI account ID.
Set META_API_TOKEN to your MetaAPI token.
Set META_API_REGION to your MetaAPI region (new-york, london, singapore).
Set LUNAR_CRUSH_API_KEY to your LunarCrush API Key.
Set MY_FX_BOOK_USERNAME to your MyFxBook username/email.
Set MY_FX_BOOK_PASSWORD to your MyFxBook password.
Set FCS_API_KEY to your FCS API KEY.
10. Allowlist Plugin
In your .env search for ALLOWLISTED_PLUGINS and add this Plugin:

################################################################################
### ALLOWLISTED PLUGINS
################################################################################
#ALLOWLISTED_PLUGINS - Sets the listed plugins that are allowed (Example: plugin1,plugin2,plugin3)
ALLOWLISTED_PLUGINS=AutoGPTMetaTraderPlugin
11. Review Available Commands

You can review the available commands and indicators here.

🧪 Test the Auto-GPT MetaTrader Plugin
Experience the plugin's capabilities by testing it for placing trades, managing your account, closing trades, and fetching candlestick data.

Test Fetching Candlestick Data
1.Configure Auto-GPT: Set up Auto-GPT with the following parameters:

Name: TradeGPT
Role: fetch candlestick data
Goals:
Goal 1: fetch candlestick data for the 1 hour chart on EURUSD
Goal 2: Terminate

2.Run Auto-GPT: Launch Auto-GPT, which should use the MetaTrader plugin and it should load the candlestick data.

3.Sample response:

<img width="320" alt="trading using gpt photo" src="https://github.com/user-attachments/assets/814a0c30-b8e0-47bb-a2ec-01df579b992c">

auto-gpt-email-plugin

📉 Indicators (In-Progress):

* Relative Strength Index (RSI)
* Volume
* Moving Averages (SMA, EMA, WMA, MAE, OsMA, MACD)
* Fibonacci Retracement
* Bollinger Bands
* Money Fund Index (MFI)
