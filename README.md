# LondonCloseEA
The files provided in this repository were developed based on the LondonClose Trading System as presented in the thread at Forex Factory (https://www.forexfactory.com/showthread.php?t=598223).  The approach was created by GhostRider.  Please refer to the link for more information on the LondonClose Trading System.

The file xm7_smLondonCloseFiboZones_v7.ex4 is the indicator

The file xm7_LondonClose_v19.ex4 is the Expert Advisor(EA)

For information on use please see following videos.  If you missed something on first video then check out the second one.  It contains a little more detail.  Video 1 is after release of version 19 and video 2 is after release of verion 16 (which at the time I thought would be the final release :) ).  I included a 3 video which shows how to use the logs and charts when in debug and verify that the EA is working.   I did this already many times but if you want to verify anthing that you think should of happened then Video 3 should give you the info you need.

Video 1: 
https://www.youtube.com/watch?v=63LOP6rlNuU

Video2: 
https://www.youtube.com/watch?v=MuYmseb2hOM

Video3 (This video shows you how use the logs and charts when in debug): 
https://www.youtube.com/watch?v=PT2SvlEHJhI

Video4:(setting up VPS time to match local PC time):
https://www.youtube.com/watch?v=cl8bNTT2uZo

The idea of creating these MetaTrader 4 tools came about cause I saw a need to develop something that was simple and straight forward.  There is a section in the LondonClose thread where SwingMan introduces his indicator(smLondonCloseFiboZones_v6.ex4). While he did a great job impleneting it, I saw alot of folks asking questions on how to setup it up.  In particular many had problems understanding the concept of GMT.  In addition an EAs that were presented only allowed the user to trade one pair at a time.  So the result was that the user would have to add the EA to MANY symbols thereby causing a possible slowdown to the MetaTrader platform.

Originally I had already started to build my EA and updated the mLondonCloseFiboZones_v6.ex4 exe but due to other projects I left it alone.  Now today I returned and in a matter of hours I completed the project.  That was the easy part.  Then came the debugging.  It took some time to get the bugs out (I would say like 2 months).  

As time permits I may be adding new features.  These are features that are not really needed but provide enhancements that will help users to work with the EA.  When updates are made, they will be anounced in the thread.

And as always.....
The material presented here is for educational purposes.  The author makes no claim as to the profitability of subject programs.  Trading involves risk, please consult a professional for guidance on these matters. 
