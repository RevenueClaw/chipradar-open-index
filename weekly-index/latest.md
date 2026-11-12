<!-- ChipRadar Edge AI & SBC Price Index — 2026-W46 -->
<!-- Generated: 2026-11-11T23:03:36.473200Z -->
<!-- Data provenance per figure: price_history (7-day windowed change), vendor_comparison vs msrp_catalog (below-MSRP deals), v_api_llm_benchmarks (LLM perf/$ and perf/W leaders) -->

# ChipRadar Edge AI & SBC Price Index — 2026-W46

**Published:** 2026-11-11T23:03:36.473200Z  
**Source of truth:** vendor-listed prices only. Amazon prices are excluded. All percentages and leaderboards are computed from the ChipRadar database.

---

## 1. 7-Day Price Movers

_No reliable 7-day price changes found in the current database snapshot. Price-history depth is too thin to compute trailing-7-day movers._

---

## 2. Boards Priced Below MSRP

_No vendor prices currently sit below documented MSRP. This can happen when stock is tight or MSRP records are missing._

---

## 3. Edge-LLM Leaderboard

### ~8B-class

- **Best tokens/$:** Jetson Orin Nano Super 8GB running **Qwen2.5 7B** @ 21.8 tok/s — 0.0873 tok/s/$ ($249.00, MLC API).

---

## 4. Raw Data Snippets

```bash
# Current vendor deals (paid API tier)
curl -H "Authorization: Bearer $CHIPRADAR_API_KEY"   https://chipradar.io/api/v1/deals

# Cited hardware LLM benchmarks (paid API tier)
curl -H "Authorization: Bearer $CHIPRADAR_API_KEY"   https://chipradar.io/api/v1/benchmarks/llm
```

MCP server configuration:

```json
{
  "mcpServers": {
    "chipradar": {
      "command": "npx",
      "args": ["-y", "mcp-chipradar@latest"],
      "env": {"CHIPRADAR_API_KEY": "YOUR_API_KEY_HERE"}
    }
  }
}
```

---

*This index is generated automatically from the ChipRadar database. Review before sharing.*
