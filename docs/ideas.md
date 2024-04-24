## Background
Possible APIs
- https://www.alphavantage.co/
	- seems to be free
- yahoo
	- https://query1.finance.yahoo.com/v7/finance/download/BAC?period1=1555274545&period2=1713127335&interval=1mo&events=history&includeAdjustedClose=true
CAPM
- [Wiki Article](https://en.wikipedia.org/wiki/Capital_asset_pricing_model)
- 
Farma French 3-Factor Model
- [Journal of Financial Economics](https://www.sciencedirect.com/science/article/pii/0304405X93900235)
[Economic Indicators](https://www.investopedia.com/ask/answers/what-are-leading-lagging-and-coincident-indicators/)
- Leading Indicators
	- Yield Curve
	- New Housing Start
	- Purchasing Manager Index
	- Money Supply
- Lagging Indicators
	- CPI
- Coincident Indicators
	- GDP

## Approach
Questions
1. Can the market and individual stocks be explained by changes in economic indicators?
	- Can asset prices  be explained by indicators from a previous year?
	- Does rate of change have a reliable impact?
2. Can the market and individual stocks be explained by consumption in different sectors?
	-  Is the impact driven by changes or rate of change?
	- Sort by industry?
3. How about consumption - production? 
4. Effect of import/exports?
5. Do Beta's that change linearly with time better explain asset values?
	- May reflect improvements in infrastructure or technology 
Road map
1. Replicate the formulation of CAPM to verify understanding
	- Can we build a monthly model and a yearly model?
2. Replicate the formulation of the FF3F model to verify understanding
	- How did FF validate their model? This will be used to validate future models.
3. Check impact of economic indicators on market
4. Build index portfolios of industries
5. Check impact of consumption on different industries
6. 