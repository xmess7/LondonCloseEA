# LondonCloseEA

IMPORTANT: If you see a wierd number for the GMT time or MARKET CLOSED when its not.  Remove the globals (F3 and delete any global that starts with xm7) and reload the EA.  

The files provided in this repository were developed based on the LondonClose Trading System as presented in the thread at Forex Factory (https://www.forexfactory.com/showthread.php?t=598223).  The approach was created by GhostBiker.  Please refer to the link for more information on the LondonClose Trading System.

The file xm7_smLondonCloseFiboZones_vXX.ex4 is the indicator

The file xm7_LondonClose_vXX.ex4 is the Expert Advisor(EA)

For information on use please see following videos.  Video 1 provides details on inputs, operation, and debugging EA operation.  Video 2 provides instructions on setting your VPS clock(some users had issues with this).

Video 1:
https://www.youtube.com/watch?v=AORXX5OYo8I

Video2:(setting up VPS time to match local PC time):
https://www.youtube.com/watch?v=cl8bNTT2uZo

The idea of creating these MetaTrader 4 tools came about cause I saw a need to develop something that was simple and straight forward.  There is a section in the LondonClose thread where SwingMan introduces his indicator(smLondonCloseFiboZones_v6.ex4). While he did a great job impleneting it, I saw alot of folks asking questions on how to setup it up.  In particular many had problems understanding the concept of GMT.  In addition other EAs that were presented only allowed the user to trade one pair at a time.  So the result was that the user would have to add those EAs to MANY symbols thereby causing a possible slowdown to the MetaTrader platform or dare I say, more confusion LOL.

I had already started to build this EA and updated the LondonCloseFiboZones_v6.ex4 indicator but due to other projects I left it alone.  Now today I returned and in a matter of hours I completed the EA and indicator.  That was the easy part.  Then came the debugging.  It took some time to get the bugs out (I would say like 2 months).  The bugs where not EA related, the bugs were mainly from the MT servers.
Yes, that is correct, the data the MetaTrader servers where providing was incorrect.  Turns out that you have to query the servers several times until the correct information (time,price) is delivered.  Why did this happen?  This happens cause you are attempting to get candle data for a symbol which is not on the chart you currently have open.   I tried several of the functions that MetaTrader provides and which each, it was the same, you have to check the data and make sure it is correct.  This is what took a while to fix and it was.  Hence when you set the debug input to true, the EA will print many of the important data results (Fibs, ATRs, etc) that it "sees" for each pair as it is looping thru the list that the user provided in the trade pairs input.  The video illustrates how you can use this information to definitely confirm if the EA is properly assessing each of the pairs. 

As time permits I may be adding new features.  These will be features that are not really needed but provide enhancements that will help users to work with the EA.  When updates are made, they will be anounced in the thread.

Jess

And as always.....
The material presented here is for educational purposes.  The author makes no claim as to the profitability of subject programs.  Trading involves risk, please consult a professional for guidance on these matters. 
