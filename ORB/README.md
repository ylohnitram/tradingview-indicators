# CCE - ORB Indicator for TradingView

**CCE - ORB** is a Pine Script indicator for TradingView that visualizes the **Opening Range Breakout (ORB)** and its extensions, including a middle line and optional VWAP. It is designed to be clear, flexible, and suitable for different trading strategies.

---

## Features

- **ORB High/Low** – displays the high and low of the opening range.
- **ORB Extensions** – visual projections of price levels above and below the ORB.
- **Middle ORB Line** – a thin gray line across the center of the range for easy reference.
- **VWAP** – optional Volume-Weighted Average Price for quick orientation.
- **Gray Fill** – shaded area between ORB high and low for better visualization.
- **Time Filters** – display only during the morning session or until the afternoon.
- **Dynamic Updates** – all lines extend automatically to the current bar.
- **Today-Only Display** – the indicator only plots for the current trading day.

---

## Installation

1. Open TradingView.
2. Go to the `Pine Editor` at the bottom.
3. Copy the `CCE - ORB` script into the editor.
4. Click `Add to Chart`.

---

## Inputs / Settings

### ORB Settings
- **ORB total time (minutes)** – duration of the opening range.
- **ORB Session Time** – specify the start and end time of the ORB session.
- **Show Extension Levels** – toggle extension lines on/off.

### Session Display
- **Display Sessions** – choose `Morning Only` or `Till Afternoon`.
- **Morning End Hour** – hour at which the morning session ends.
- **Afternoon End Hour** – hour at which the afternoon session ends.

### VWAP Settings
- **Show VWAP** – toggle VWAP display on/off.
- **Source** – price source for VWAP calculation.

---

## Notes

- The indicator updates dynamically as new bars are formed.
- VWAP is only plotted for the current session and for today’s bars.
- The middle ORB line is aligned with the center of the range and extends across the gray fill.
- Works best on intraday timeframes.

---

## License

MIT License – feel free to use, modify, and share.

---

## Author

CCE_Charts  
GitHub: ylohnitram
