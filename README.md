# +EV Engine — Live Track Record

Automated edge detection across Kalshi prediction markets and major US sportsbooks. Every pick is posted to Discord **before first pitch** — Discord timestamps are immutable and publicly verifiable.

## Dashboards

- **[Kalshi Props](props.html)** — pitcher strikeout props, Kalshi price vs. sportsbook consensus, CLV tracked on every bet
- **[Sportsbook Gaps](sportsbook.html)** — MLB/NHL moneyline/spreads/totals, soft books vs. sharp anchor, Kelly-sized paper bets

## How edge is proven

**CLV (Closing Line Value)** is the primary metric — not win rate.

If you consistently get a better price than where the market closes, you're systematically beating the most efficient estimate of true probability. That's the definition of edge, and it's provable 3–5× faster than waiting for ROI to converge.

Target: beat-the-close > 63% at n=50, > 57% at n=200 (p<0.05, one-sided binomial).

## Methodology

- **Sharp anchor**: Pinnacle / LowVig (lowest-vig books, closest to true probability)
- **De-vig**: 2-way no-vig to strip the hold and get fair probability
- **Staking**: ¼ Kelly, capped at 5 units, fee-adjusted for Kalshi contracts
- **Props anchor**: sportsbook consensus (FanDuel/DraftKings) — softer than Pinnacle, edges are thinner
- **Freshness gate**: stale sharp data (>10 min) filtered before alerting

## Disclaimer

Educational data only. Paper trades — no real money. Not financial or betting advice.
