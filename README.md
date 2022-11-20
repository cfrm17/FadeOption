# FX Fade Option Valuation

So-called “fade option” can be more precisely named as “point-barrier option”. The fade option is a vanilla option that exists or dies if a barrier is breached on a single preset date, which is prior or equal to the contract maturity. Therefore, the barrier type can be up-cross or down-cross; the exercise type can be knock-in or knock-out; and the underlying vanilla can be call or put.

Let 0 < T1 · T2 · T, K > 0 and h ¸ 0. Let us define the barrier knock type index as

 

and the exercise type index as

 

as well as the underlying vanilla option type index as

 

Finally, define a function of H on (0;1) with any given (knock; exType; h) as

 

The point-barrier option can be defined as follows. Let fSt : t ¸ 0g be the (strictly positive) price process of the underlying asset, T1 be the point barrier time, h be the single barrier, K be the underlying vanilla option strike, T2 be the option maturity, and T be the option payoff time. Then the matured payoff at T of the option, denoted by VT , can be given by

 

It should be noticed that for ST1 with continuous distribution, the probability of an event fST1 = sg is always zero for any s > 0. Hence, in the definition of the function H, the inequality (¸) and the strict inequality (>) can be inter-changeable with no effect on the initial value of the option.

There are four types of single point-barrier options and they are Up-In, Up-Out, Down-In, and Down-Out. A double point-barrier option can be easily composed of two single point-barrier options. Let 0 · hL <hU · 1. First, we have

 
 

Let If¢¢¢ g be the indicate function. For [hL; hU]-Knock-In, we have

 

i.e., it is equal to one Down-In minus another Down-In or one Up-In minus another Up-In. Similarly, for (hL; hU)-Knock-Out, we have

 

i.e., it is equal to one Down-In plus one Up-In. Therefore, it suffices to consider single point-barrier options.

We assume that the zero-coupon bond price (see https://finpricing.com/lib/FiBond.html )

 

can be used as the numeraire for the market such that, under the equivalent martingale measure N with
respect to the numeraire N, the dynamics of the underlying price can be given by

 

where F0(¢) is the initial forward price of the underlying asset, WN is the standard Wiener process under
N and ¾ is the volatility of S which can be implied by market term volatilities of vanilla options of the
underlying asset, i.e., we have

 

Then the initial value of the option, denoted by V0, can be given as

 
