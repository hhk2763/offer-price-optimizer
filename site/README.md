# Offer Price Optimizer

**Case study:** https://hhk2763.github.io/offer-price-optimizer/
**Full-screen app:** https://hhk2763.github.io/offer-price-optimizer/app.html

This is a pricing desk I built for an aviation parts broker. It's a Google Apps Script web app that runs on top of the broker's existing Google Sheets. A buyer picks a part and pins three of five numbers: sale price, overhaul (OH) cost, offer, markup and gross profit. The tool solves the other two. Pinning sale price, OH cost and a target markup, for example, gives the most the buyer can offer for the part.

- **Solver:** GP = Sale − Offer − OH cost, and Markup = GP ÷ (Offer + OH cost). Pin any 3 and it solves the other 2.
- **Repair quotes as inputs:** click a repair station's quote to use it as the OH cost. Compare up to 4 scenarios, then lock one.
- **One link per deal:** a Config tab points the app at a deal workbook. Columns are matched by name, so different sheet layouts work.
- **Scenarios log:** locked prices are written to a Scenarios tab and restored when the page reloads.

The client is anonymised. The version in this repo runs on fictional part numbers, suppliers and prices, with an in-browser stand-in for the Apps Script backend, so it works as a static page.

Built by Huma · Google Sheets, Apps Script, HTML/JavaScript
