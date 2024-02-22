# DexScreenerAlerts
A script that gets data of defi crypto pairs from dexscreener, and sends it to a telegram channel.

### Sample pair.txt file:

- If a line contains a dexscreener pair code, the script will print its price and 24hr changes.
- If a ", i" is appended to the end of the pair code, the pair will be inversed (e.g. BTC/USD to USD/BTC)
- Otherwise, print normally.

Script is regularly run on AWS Lambda, scheduled through EventBridge (Cloudwatch Events).

