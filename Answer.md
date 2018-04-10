# StatMech Assignment 1

## Name: Zheng-Lin Tsai             &ensp; ID: s106022501

## Problem 0: One die with 6 sides

1. my code: [OneDice.cpp](OneDice.cpp)

2. 
3. 
    
    | sides |   N_s   |   N_s-N/6 | N_s/N    | N_s/N-1/6 |
    |-------|:-------:|----------:|----------|-----------|
    | 1     | 8333075 |  258.3333 | 0.166661 | 0.000005  |
    | 2     | 8336919 | 3585.6667 | 0.166738 | 0.000072  |
    | 3     | 8332031 | 1302.3333 | 0.166641 | 0.000026  |
    | 4     | 8333177 | 156.3333  | 0.166664 | 0.000003  |
    | 5     | 8332071 | 1262.3333 | 0.166641 | 0.000025  |
    | 6     | 8332727 |  606.3333 | 0.166655 | 0.000012  |

    Number of trials: 50000000, and time spent: 1 sec

4. In my code, the N_s/N-1/6 whole decrease.

5. Yes, N_s/N approach closer to 0.166667 (1/6), at 50000000 trials the error is 0.004%

## Problem 1: One die with S sides

1. my code: [OneDiceS.cpp](OneDiceS.cpp)

2. Example 8-sides at 50000000 trials.

    | sides |     N_s |   N_s-N/S |    N_s/N | N_s/N-1/S |
    |------:|--------:|----------:|---------:|----------:|
    |     1 | 6249159 |  841.0000 | 0.124983 |  0.000017 |
    |     2 | 6250176 |  176.0000 | 0.125004 |  0.000004 |
    |     3 | 6254336 | 4336.0000 | 0.125087 |  0.000087 |
    |     4 | 6252052 | 2052.0000 | 0.125041 |  0.000041 |
    |     5 | 6247210 | 2790.0000 | 0.124944 |  0.000056 |
    |     6 | 6247691 | 2309.0000 | 0.124954 |  0.000046 |
    |     7 | 6250770 |  770.0000 | 0.125015 |  0.000015 |
    |     8 | 6248606 | 1394.0000 | 0.124972 |  0.000028 |

    mean: 4.4997432, variance: 5.2496581, standard deviation: 2.2912132

    **** Check by theoretical prediction ****

    mean: 4.5, variance: 5.252311, standard deviation: 2.2917921

    **** Check error ****

    mean error: 0.0057062222%, variance error: 0.050507672%, standard deviation error: 0.025257026%.


    Number of trials: 50000000, and time spent: 1 sec

3. I take 8-sides and 7-sides dice, and trials 10000000 times.

    | sides |     N_s |   N_s-N/S |    N_s/N | N_s/N-1/S |
    |------:|--------:|----------:|---------:|----------:|
    |     1 | 6249159 |  841.0000 | 0.124983 |  0.000017 |
    |     2 | 6250176 |  176.0000 | 0.125004 |  0.000004 |
    |     3 | 6254336 | 4336.0000 | 0.125087 |  0.000087 |
    |     4 | 6252052 | 2052.0000 | 0.125041 |  0.000041 |
    |     5 | 6247210 | 2790.0000 | 0.124944 |  0.000056 |
    |     6 | 6247691 | 2309.0000 | 0.124954 |  0.000046 |
    |     7 | 6250770 |  770.0000 | 0.125015 |  0.000015 |
    |     8 | 6248606 | 1394.0000 | 0.124972 |  0.000028 |

    mean: 4.4994021, variance: 5.2500378, standard deviation: 2.2912961

    **** Check by theoretical prediction ****

    mean: 4.5, variance: 5.2553807, standard deviation: 2.2924617

    **** Check error ****

    mean error: 0.013286667%, variance error: 0.10166533%, standard deviation error: 0.05084559%.


    Number of trials: 10000000, and time spent: 0 sec
    
 
    | sides |     N_s |   N_s-N/S |    N_s/N | N_s/N-1/S |
    |------:|--------:|----------:|---------:|----------:|
    |     1 | 1429769 | 1197.5714 | 0.142977 |  0.000120 |
    |     2 | 1428923 |  351.5714 | 0.142892 |  0.000035 |
    |     3 | 1428135 |  436.4286 | 0.142814 |  0.000044 |
    |     4 | 1428298 |  273.4286 | 0.142830 |  0.000027 |
    |     5 | 1427343 | 1228.4286 | 0.142734 |  0.000123 |
    |     6 | 1428538 |   33.4286 | 0.142854 |  0.000003 |
    |     7 | 1428994 |  422.5714 | 0.142899 |  0.000042 |
        
    mean: 3.9996113, variance: 4.0014187, standard deviation: 2.0003547

    **** Check by theoretical prediction ****

    mean: 4, variance: 4.0031094, standard deviation: 2.0007772

    **** Check error ****

    mean error: 0.0097175%, variance error: 0.042234668%, standard deviation error: 0.021119564%.


    Number of trials: 10000000, and time spent: 0 sec

4. At 10000 trials, I got mean error: 0.052666667%, standard deviation error: 0.062527559%.

   But, this case (10000 trials) the result can less than 1%. Next time maybe cannot less than 1%.
   Then I try to do 1000 times 2000 trials, and get more general error.
   
   data : 
   
   mean error: 0.0106%, standard deviation error: -0.26545938%.
   
