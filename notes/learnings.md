### Data Structure

### BBO (Best Bid and Offer)
Observations from bbo information:
| Column Name | Type | Example | Description |
|------------|------|---------|-------------|
| `timestamp` | datetime (μs, Asia/Singapore) | `2026-04-09 13:00:00.013 +08` | Timestamp in Singapore timezone with millisecond/microsecond precision |
| `exchange` | String | `binance` | Name of the cryptocurrency exchange |
| `symbol` | String | `BTC-USD-PERP` | Trading instrument symbol (Bitcoin USD perpetual futures) |
| `bid_price` | Float64 | `70760.0` | Highest buying price currently available |
| `bid_size` | Float64 | `21.519` | Quantity available at the highest bid price |
| `ask_price` | Float64 | `70760.1` | Lowest selling price currently available |
| `ask_size` | Float64 | `6.505` | Quantity available at the lowest ask price |
| `local_timestamp` | i64 | `` | Check for nullity in data |
| `date` | Date | `2026-04-09` | Verify relation to timestamp |
 

Symbols present in bbo:
| Symbol | Description |
|---|---|
| `BTC-USD-PERP` | Bitcoin/USD Perpetual |
| `BTC-USD-SPOT` | Bitcoin/USD Spot |
| `SOL-USD-PERP` | Solana/USD Perpetual |
| `SOL-USD-SPOT` | Solana/USD Spot |
| `ETH-USD-PERP` | Ethereum/USD Perpetual |
| `ETH-USD-SPOT` | Ethereum/USD Spot |


Running To Do:
- what does this timestamp mean?
