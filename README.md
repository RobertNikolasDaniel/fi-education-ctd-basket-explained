# CTD Baskets, Convexity, and Yield Curve Trades

A simple educational presentation exploring why Treasury futures curve trades are not just duration trades—they are also CTD basket and convexity trades.

---

## Overview

When traders build a Treasury futures relative value (FIRV) trade, they often focus on:

- Duration
- DV01
- Yield curve exposure

However, every Treasury futures contract references a **Cheapest-to-Deliver (CTD) basket**, and each basket contains securities with different duration and convexity characteristics.

As a result, two futures contracts can react differently to the same yield curve move, even when the trade appears DV01-neutral.

---

## Core Idea

```text
Treasury Futures
        ↓
   CTD Basket
        ↓
    Convexity
        ↓
 Yield Curve P/L
```

The CTD basket determines the bond exposure ultimately driving futures behavior.

Different baskets create different convexity profiles.

---

## Why It Matters

A yield curve trade is not always:

```text
Short 5Y
Long 10Y
```

In practice, it is often closer to:

```text
Short 5Y CTD Basket
Long 10Y CTD Basket
```

Since the baskets differ, so do:

- Duration
- Convexity
- Financing
- Delivery economics

These differences can create unexpected P/L during large yield curve moves.

---

## Convexity Divergence

Convexity measures how bond duration changes as yields move.

Higher convexity generally means:

- Larger gains during rallies
- Smaller losses during selloffs

Lower convexity generally means:

- More linear price behavior
- Less curvature in price response

Because CTD baskets contain different securities, they naturally contain different convexity exposures.

This creates:

```text
Convexity Divergence
```

between Treasury futures contracts.

---

## Rich vs Cheap Futures Curves

The presentation includes simplified examples showing:

- Rich futures curves
- Cheap futures curves
- Market futures prices
- Ideal futures prices derived from spot markets

```text
Market Futures > Ideal Futures
                ↓
              Rich

Market Futures < Ideal Futures
                ↓
              Cheap
```

---

## Main Takeaway

Treasury futures are not simply duration products.

They are a combination of:

- Cash bonds
- Repo financing
- Delivery optionality
- CTD basket selection
- Convexity exposure

Understanding CTD baskets helps explain why seemingly similar Treasury futures can produce very different outcomes during yield curve trades.

---

## Lessons Learned

One of the biggest realizations from building Treasury futures projects is:

> A yield curve trade is not just a yield curve trade.

The underlying CTD basket can materially affect how a futures position behaves.

This is one reason Treasury futures relative value trading is often more complex than simply comparing two points on the Treasury curve.

---

## Educational Purpose

This presentation was created as a student learning exercise to better understand:

- Treasury futures
- CTD baskets
- Relative value trading
- Yield curve positioning
- Convexity effects
- Futures versus cash market relationships

The goal is educational intuition rather than production trading analytics.

---

## Related Projects

- Student CTD Finder
- Student Treasury Futures Basis Calculator
- Student Carry vs Market Analyzer
- Student Invoice Price Calculator
- Student Treasury Curve Workstation
- Student CTD vs CME Convexity Shock Graph

---

### Simple. Honest. Useful.

Built as part of an ongoing series of educational Treasury futures and fixed income projects.
