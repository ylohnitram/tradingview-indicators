CCE - ORB Indicator
Professional Pine Script indicator for Opening Range Breakout (ORB) strategies with automatic US market session detection and advanced features.

🚀 Features
✨ Core Features
Automatic US market open detection (9:30 AM ET) - no manual time configuration needed

Flexible ORB duration - set any number of minutes (5, 15, 30, etc.)

Extension levels - automatic 0.5x, 1x, 1.5x ORB range calculations

VWAP integration - resets at ORB session start

Gray fill between ORB high/low for better visualization

Universal alert for all ORB level breaches

📊 Displayed Levels
ORB High/Low - main support/resistance levels (gray lines)

Midline - center of ORB range (gray dashed)

Extension levels:

0.5x (light green/red)

1x (medium green/red)

1.5x (dark green/red)

VWAP - volume weighted average price (green/red based on position)

⚙️ Settings
ORB Settings
Parameter	Description	Default Value
ORB Duration	Length of ORB session in minutes	15 minutes
Show Extension Levels	Show/hide extension levels	Enabled
Session Settings
Parameter	Description	Options
Display Sessions	When to display ORB levels	Morning Only / Till Afternoon
Morning Only: 9:30 AM - 12:00 PM ET

Till Afternoon: 9:30 AM - 4:00 PM ET

VWAP Settings
Parameter	Description	Default Value
Show VWAP	Show/hide VWAP	Enabled
Source	Data source for VWAP calculation	HLC3
🕒 Timing
Automatic US Market Hours Detection
The indicator automatically detects:

Market Open: 9:30 AM Eastern Time

ORB Session: 9:30 AM + specified duration (e.g., 9:30-9:45 for 15min ORB)

Morning Session: 9:30 AM - 12:00 PM ET

Afternoon Session: 12:00 PM - 4:00 PM ET

Timezone Handling
Everything runs on America/New_York timezone

Automatic EST/EDT switching (daylight/standard time)

Independent of your local timezone

📈 Indicator Behavior
ORB Lines (gray lines)
Start: From ORB session beginning (e.g., 9:30)

Display: All day according to Session Settings

Update: Dynamically extend to current bar

VWAP (green/red line)
Resets: At ORB session start (9:30)

Displays: Only after ORB session ends (9:45)

Color:

🟢 Green = Close > VWAP

🔴 Red = Close < VWAP

⚪ Invisible = outside valid session or before ORB completion

Gray Fill
Fills space between ORB High and ORB Low

Shows only in most recent session (last ~300 bars)

85% transparency for better readability

🚨 Alerts
Universal Alert for All ORB Levels
One alert covers breaches of all levels:

ORB High/Low

Midline

All Extension levels

Alert triggers on:

Breach of any ORB level in either direction

Only on new breaches (not continuously)

Only when ORB levels are active

Alert message: "Price breached an ORB level: {ticker} at {close}"

🎯 Usage
For Day Trading
Set ORB duration according to your strategy (typically 15-30 minutes)

Watch for first breach of ORB High/Low after 9:45 AM

Use Extension levels as profit targets

VWAP as filter - long positions above VWAP, short below VWAP

For Swing Trading
Set "Till Afternoon" for full trading day

Use Extension levels for larger price targets

VWAP trend as long-term direction

For Backtesting
Indicator works correctly in Replay mode

Gray fill and VWAP display only in current period

Lines remain visible throughout history

🔧 Installation
Open Pine Script Editor in TradingView

Delete default code and paste the complete indicator code

Click "Add to Chart"

Configure parameters according to your needs

📋 Compatibility
Pine Script v5

Timeframes: All intraday timeframes (1m, 5m, 15m, etc.)

Symbols: US stocks and ETFs with trading hours 9:30-16:00 ET

TradingView: All account types

❗ Important Notes
Works only on US market symbols (NYSE, NASDAQ)

Requires intraday timeframe for proper function

VWAP resets daily at ORB session start

Extension levels are calculated based on ORB range (high-low)

🤝 Support
For questions, bug reports, or suggestions, please create an Issue in this repository.

⚡ For best results, use on 5M or 15M timeframe with US stocks.
