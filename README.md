# Global Arms Transfer Network Analysis

A Python tool for visualising how the global arms trade network has evolved over time, using data from the [SIPRI Arms Transfers Database](https://www.sipri.org/databases/armstransfers).

## Overview

This script builds directed trade graphs for three time periods and renders them as network visualisations. Edge width reflects the SIPRI Trend Indicator Value (TIV) of each supplier→recipient relationship, so the heaviest arms flows stand out visually. Each period also prints a summary of node count, edge count, and network density — making it easy to see whether the global arms market is expanding or consolidating.

## Output

For each period the script produces:
- A high-resolution network image (`network_1995-2000.png`, etc.)
- A console summary: `2005–2010: 55 countries, 91 trade links, density=0.031`

## Time Periods

| Period | Focus |
|--------|-------|
| 1995–2000 | Post-Cold War restructuring |
| 2000–2005 | Pre-9/11 and early War on Terror |
| 2005–2010 | War on Terror era demand |
| 2010–2015 | Arab Spring and regional instability |
| 2015–2020 | Rise of new arms importers |
| 2020–2025 | Contemporary transfers |

## Requirements

```bash
pip install networkx matplotlib pandas numpy
