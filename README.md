# Kc_updown_3bar_BOTH
Strategy

If fibbar very big and then the bar after that is smaller but pivots the other way,
	//then the bar after that retraces into the 2ndbars body/open and bounces from there and heads the other way,
	//then breaks the extremity of the 2ndbar, confirming the move: we enter into the trade in that direction.
	//We look for a BIG profit and this is not a lofty dream target. 
	//Due to the size of the fibbar it signifies a shake-out of stops, and then the confirmaiton that it is going back
	//to the mean(or possibly more) is shown. 
	//The reason I don't have my target at the beginning of the fibbar is because when it comes back that quick, 
	//HTF's probably show a hammer or something, but if it gets to the fibbar open, it is likely going to go more. 
	//Pick big targets and cut losses short. You will lose much more than win, but this is a signal that trend has changed.

 { requirements:
	bullfib(Noplot atr req).
	2ndbar(Close < open, high can be higher or lower than bullfib high. , bottomwick > upperwick, 
	3rdbar(high > close[1], high < higher of bullfibhigh or high of 2ndbar., 
	If breaks low enter. 
}
//If the 3min is what you say it is...identifys free space unlike the HTF because there's smaller zones inside the HTF free space,
//the 3min should have no excuses but to be free space. It is the smallest timeframe needed. 

//Works the BEST if the entrybar actually touches the open and nothing more, nothing less. So it grabs the 2ndbar open and turns down and breaks low, that is the signal!
//Test with making the bullfib have a ACB or ATR requirement. (my guess is ATR+1SD shows increase in volatility which makes us think our chart pattern will work bc it needs a movement back to the mean., idk.


{Add-ons:
	Only take trades if the freespace is big. Only if risk < reward. Backtest must win over 50% and we're in good!
	Only trade 8-3
	Maybe you could add-on to the bar before the bullfib-- make sure it is a base and that it isn't a solid body move.
	}
