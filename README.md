EAT MY SHORTS

Developed by Oliver Leiriao & Ravi Raina

How did r/wallstreetbets discover an opportunity to trap greedy hedge funds and realize unbelievable returns? 
By looking at a few key statistics publicly available, one can get an approximate idea of how bad a company's stock is being shorted, how long until that short position comes due, and how likely, given the current stock price's fluctuations, an individual investor can realize a quick and significant (albeit, risky) gain.

We used a Yahoo Finance API to pull stock info, React for the frontend, Flask for the backend, and Docker and AWS for deployment.


Stonk info used:

* Short Interest Ratio:
    Often used to gauge investor sentiment regarding the company, it is also quick way to see how heavily shorted a stock may be versus its recent trading volume. Most importantly  it can be an indication of how many days it would take for all the shares short to be covered or repurchased in the open market (aka Days To Cover).

* Short % of Float:
    The percentage of short positions on a stock as part of the total publicly available stock not held by insiders or institutions. This is also a harbinger of stocks that are in truly bad shape.

* Daily Avg. Trade Volume (10-Day):
    The average number of positions of a stock traded in a day, on a 10 day average. If this is low as a short position is coming due, it could factor into what may potentially be a short squeeze opportunity.

* Short Term Trend:
    If a stock is trending up as a short position is coming due, it could factor into what may potentially be a short squeeze opportunity.


The stock is given a score and is graded on 9 based on ratio ranges we set. 
The app posts statistics along with one of three messages: there is a potential short squeeze opportunity, there is no opportunity (the stock's ratios are healthy) or there is no way of knowing one way or the other.


* Disclaimer: we are not financial advisors. None of the information this platform provides should be taken seriously, nor should it be used to make investment decisions.
