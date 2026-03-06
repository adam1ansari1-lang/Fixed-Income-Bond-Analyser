# Fixed-Income-Bond-Analyser
What This Project Does
This project is a quantitative fixed income analysis tool built in Python. It prices bonds, calculates yields, measures risk, and visualises how bonds behave when interest rates change — all from scratch using real financial mathematics.

Concepts Covered
Discounted Cash Flow (DCF) Pricing — every bond is priced by discounting its future cash flows back to today using the market yield as the discount rate. This is the foundational model used across all of fixed income finance.
Yield to Maturity (YTM) — rather than rearranging the DCF formula algebraically (which is impossible), the tool uses Brent's Method — a numerical root-finding algorithm — to solve for the yield that justifies any given market price. This is a genuine quantitative technique used in practice.
Modified Duration — measures how sensitive a bond's price is to a 1% change in yield. A bond with a modified duration of 7.5 will lose approximately 7.5% of its value if yields rise by 1%. This is the primary risk metric used by fixed income traders.
Convexity — captures the curvature of the price/yield relationship that duration alone misses. Because convexity is always positive for standard bonds, prices rise more when yields fall than they fall when yields rise by the same amount — an asymmetry that is genuinely valuable to bondholders.
Rate Shock Analysis — combines duration and convexity into a second-order approximation formula to estimate price changes across a range of yield shocks from -300 to +300 basis points, comparing the estimate against exact DCF repricing.

