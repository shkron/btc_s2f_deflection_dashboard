# Bitcoin Stock-to-Flow (S2F) Dashboard

An interactive dashboard for exploring Bitcoin’s **Stock-to-Flow (S2F) model**, spot price, and deflection ratio.  
Built with **Chart.js** and plain JavaScript (no server required).

---

## Features

- **BTC vs S2F Model Chart**
  - Overlays historical BTC/USD price with the S2F model price (PlanB 2019 regression).
  - Optional **200-Week Moving Average** (200W MA) overlay that can be toggled on/off via checkbox.
  - Supports **drag-to-pan**, **wheel/pinch zoom**, **double-click reset**, and keyboard arrow panning.

- **S2F Deflection Chart**  
  - Displays the ratio *Price ÷ Model*.  
  - Includes a **pale grey dashed reference line at 1.0**.  
  - Highlights **Bitcoin halving events** with vertical dashed lines.  

- **Info Tooltips**  
  - Each chart has an ⓘ button opening a short modal explanation.

- **Summary Tiles**  
  - Shows latest spot price, current S2F value, model price, and deflection.

- **Custom Model Coefficients**  
  - Adjust parameters `A` and `B` for the regression formula:  
    ```
    ln(MV) = A · ln(S2F) + B
    ```

---

## Data Sources

- Primary: [CoinCap](https://coincap.io/)  
- Fallbacks: CryptoCompare, Binance, CoinGecko (optional API key supported)

---

## Usage

1. Save `btc_s2f_deflection_dashboard.html` locally.  
2. Open it in any modern browser (Chrome, Firefox, Edge).  
3. Use the controls to pan/zoom charts or adjust model coefficients.  
4. Click ⓘ buttons for quick chart explanations.

---

## Notes

- Annual Bitcoin issuance is calculated per halving epoch (reward × 144 blocks/day × 365).  
- Circulating supply is anchored at exact halving totals.  
- This tool is **for research and educational purposes only**; not financial advice.

---

