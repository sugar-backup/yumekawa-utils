# yumekawa-utils
Blockchain Utility Collection for Sugarchain

## Contents
 - `max_money`: check the schedule of total supply and draw graph

## Comming Soon
 - `difficulty`: check historical difficulty with blocktime and draw graph
 - `nonce`: check historical nonces and draw graph
 - `blockchain_size`: check historical total blockchain size and draw graph
 - `blocktime_RT`: check current blocktime in realtime
 - `hash_attack`: simulate hash attack
 - `getFullBlockchain`: dump all blockchain data as plain text

-----

### max_money
![](https://github.com/sugarchain-project/yumekawa-utils/blob/master/max_money/max_money.png)

 - depends
```bash
sudo apt-get install gnuplot && \
pip install numpy
```

 - run
```bash
cd max_money && \
./max_money.py && \
cat ./max_money.csv && \
gnuplot ./max_money.plot; \
cd ..
```

 - data
```
Block Time:		5 Seconds
Initial Block Reward:	4294967296 Satoshis
Initial Block Reward:	42.94967296 COINs
Halving Interval:	12614400 Blocks
* in Years:		  2 Years
* in Days:		  730 Days
* in Hours:		  17520 Hours
* in Minutes:		  1051200 Minutes
* in Seconds:		  63072000 Seconds
Total Halving Count:	33 Times
* in Years:		  66 Years
* in Days:		  24090 Days
* in Hours:		  578160 Hours
* in Minutes:		  34689600 Minutes
* in Seconds:		  2081376000 Seconds
Total Satoshis:	108356870904710400 Satoshis
Total COINs:		1083568709.047104 COINs

[ OK ]: all range check is finished

# WARNING: the first halving is NOT half of the total supply!
Total Supply:		108356870904710400
Half of Total Supply:	54178435452355200
First Halving:	54178435458662400
Difference:		-6307200 Satoshis

Count	Supply			Reward
0	0			4294967296
1	54178435458662400	2147483648
2	81267653187993600	1073741824
3	94812262052659200	536870912
4	101584566484992000	268435456
5	104970718701158400	134217728
6	106663794809241600	67108864
7	107510332863283200	33554432
8	107933601890304000	16777216
9	108145236403814400	8388608
10	108251053660569600	4194304
11	108303962288947200	2097152
12	108330416603136000	1048576
13	108343643760230400	524288
14	108350257338777600	262144
15	108353564128051200	131072
16	108355217522688000	65536
17	108356044220006400	32768
18	108356457568665600	16384
19	108356664242995200	8192
20	108356767580160000	4096
21	108356819248742400	2048
22	108356845083033600	1024
23	108356858000179200	512
24	108356864458752000	256
25	108356867688038400	128
26	108356869302681600	64
27	108356870110003200	32
28	108356870513664000	16
29	108356870715494400	8
30	108356870816409600	4
31	108356870866867200	2
32	108356870892096000	1
33	108356870904710400	0
```

### max_moneyBTC (optional)
<!-- ![](https://github.com/sugarchain-project/yumekawa-utils/blob/master/max_moneyBTC/max_moneyBTC.png) -->

 - data
```
Block Time:		600 Seconds
Halving Interval:	210000 Blocks
* in Years:		  3.995433789954338 Years
* in Days:		  1458.333333333333 Days
* in Hours:		  35000 Hours
* in Minutes:		  2100000 Minutes
* in Seconds:		  126000000 Seconds
Total Halving Count:	33 Times
* in Years:		  131.8493150684932 Years
* in Days:		  48125 Days
* in Hours:		  1155000 Hours
* in Minutes:		  69300000 Minutes
* in Seconds:		  4158000000 Seconds
Total Satoshis:	2099999997690000 Satoshis
Total COINs:		20999999.97690000 BTC

Count	Supply			Reward
0	0			5000000000
1	1050000000000000	2500000000
2	1575000000000000	1250000000
3	1837500000000000	625000000
4	1968750000000000	312500000
5	2034375000000000	156250000
6	2067187500000000	78125000
7	2083593750000000	39062500
8	2091796875000000	19531250
9	2095898437500000	9765625
10	2097949218750000	4882812
11	2098974609270000	2441406
12	2099487304530000	1220703
13	2099743652160000	610351
14	2099871825870000	305175
15	2099935912620000	152587
16	2099967955890000	76293
17	2099983977420000	38146
18	2099991988080000	19073
19	2099995993410000	9536
20	2099997995970000	4768
21	2099998997250000	2384
22	2099999497890000	1192
23	2099999748210000	596
24	2099999873370000	298
25	2099999935950000	149
26	2099999967240000	74
27	2099999982780000	37
28	2099999990550000	18
29	2099999994330000	9
30	2099999996220000	4
31	2099999997060000	2
32	2099999997480000	1
33	2099999997690000	0
```