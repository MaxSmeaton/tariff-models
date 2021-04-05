# tariff-models
FICO Xpress mosel and data files for modelling Fixed-Price and Real-Time-Pricing tariffs.


The main two files for consideration here are 'fptariff.mos' and 'rtp.mos'. These are the models for the Fixed-Price and Real-Time-Pricing model respectively. The base cases are done by having the initializations run from 'fptariff.dat' and 'rtp.dat'. 

To consider other cases the data file may be altered directly or the initializations my be done from the other files provided. If altering directly, not that the FP tariff must first be solved, and the the optimal FP payoff must be placed in the respective RTP data file in order for the models to work.

By changing the initializations to be from 'fplower.dat' and 'rtplower.dat' a lower bound case, with the same spot prices but lower sunlight hours can be seen.

'fpMAY.dat' and 'rtpMAY.dat' provide the upper-bound, uses numbers taken from May 2020, and have optimistic sunlight hours and spot prices.


For the 'no battery' case, the mosel file must be changed as this is a different model. For this example 'fptariffnobat.mos' and 'rtpnobat.mos' should be used. These files only work with the corresponding 'fptariffnobat.dat' and 'rtpnobat.dat' files which can be altered if you wish to consider alternate 'no-battery' scenarios .
