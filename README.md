# calc-tip
Restaurant Bill &amp; Tip Calculator
Restaurant Bill & Tip Calculator (v5c) — User Guide & Quick Reference
Welcome to your offline-first, group-optimized billing workspace. This guide explains how to use the calculator's advanced rounding engines, custom shortcuts, and server protection guardrails.

🚀 Quick Start Guide
Open the App using this URL:  https://kenmarlies.github.io/calc-tip/
Enter the Meal Cost: Type the base receipt subtotal (Meal + Tax) into the Meal Cost box.
Set the Rates: Adjust your credit card fee and target tip using the quick-select percentage buttons.
Split the Bill (Optional): Change the Number of People field to instantly divide the total.
Log & Clear: Click Save History to log the receipt to your sidebar, 
then click Clear to wipe the board for your next meal -or- simply modify the prior entries for another bill.

🛠️ Inputs & Advanced Controls
💳 Credit Card Surcharge Rate
Default: 0.0%
Quick Presets: 1%, 2%, 3% buttons for rapid setting.
Math Behavior: This surcharge is dynamically applied to the combined subtotal of the food and the finalized tip, perfectly mirroring modern retail merchant processors.
💰 Desired Tip Percentage
Default: 18.0% (Automatically prefilled on launch)
Quick Presets: 15%, 18%, 20% buttons.
Math Behavior: Serves as your ideal baseline target. The rounding engine will dynamically pivot off this number to secure your whole-dollar totals.
🛡️ Tip Override (Minimum Dollar Amount)
Default: $0
What it does: Acts as an unconditional cash floor for the server.
Use Case: Perfect for small bills (e.g., a $4 coffee where an 18% tip is only pennies, but you want to leave a flat $2), or if you prefer to tip a specific flat cash amount regardless of bill percentages.
👥 Number of People (Split)
Default: 1
What it does: Dictates whether the calculator targets a whole-dollar Grand Total (Party Size = 1) or a whole-dollar Per-Person Share (Party Size > 1).

🔬 How this will Protect Your Server
Traditional bill-splitting tools round down blindly, which aggressively shortchanges waitstaff as groups grow. This introduces Tip Protection Layout Metrics:
🚫 The -1.0% Downside Variance Guardrail
When splitting, the application runs a trial calculation by rounding the individual share to the closest dollar. It then cross-checks what that round does to the server's tip percentage.
If a downward round causes the Effective Tip Rate to drop more than 1.0% below your Desired Tip, the guardrail instantly overrides standard rounding.
It forces the calculation to round UP to the next whole dollar instead, preserving a fair tip for the server and keeping individual splits a clean, even number.
🛑 The Override Floor Enforcement
If a downward round attempts to drop the total tip amount below the value specified in your Tip Override box, the calculator blocks the downward slide and forces an upward round to keep that cash floor fully locked.
