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

![](https://github.com/sugarchain-project/yumekawa-utils/blob/master/max_money/excel.png)

 - depends
```bash
sudo apt-get install gnuplot && \
pip install numpy
```

 - run python
```bash
cd max_money && \
./max_money.py && \
cat ./max_money.csv && \
gnuplot ./max_money.plot; \
cd ..
```

- run C++
```bash
cd max_money && \
g++ max_money.cpp -std=c++11 -o max_money; \
./max_money; \
cd ..
```

- run java
```bash
sudo apt-get install default-jre
```
```bash
cd max_money && \
javac max_money.java && \
java max_money ; \
cd ..
```

 - data: sugarchain
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
Total Halving Count:	64 Times
* in Years:		  128 Years
* in Days:		  46720 Days
* in Hours:		  1121280 Hours
* in Minutes:		  67276800 Minutes
* in Seconds:		  4036608000 Seconds
Total Satoshis:	108356870917324799 Satoshis
Total COINs:		1083568709.173248 COINs

[ OK ]: checking range is finished

# WARNING: the first halving is NOT exactly half of the total supply!
Total Supply:		108356870917324799
Half of Total Supply:	54178435458662399
First Halving:	54178435458662400
Difference:		-1 Satoshi(s)

# INFO:
total supply '108356870917324799+1' is 108356870904710400+(63072000/10*2)'
'+1' is correction by virtual halving under 1 satoshi
108356870904710400 is 33th halving with 0 reward
63072000 is the halving interval in seconds

Count	Supply			Pow	Reward
0	0			2^{32}	4294967296
1	54178435458662400	2^{31}	2147483648	
2	81267653187993600	2^{30}	1073741824	
3	94812262052659200	2^{29}	536870912	
4	101584566484992000	2^{28}	268435456	
5	104970718701158400	2^{27}	134217728	
6	106663794809241600	2^{26}	67108864	
7	107510332863283200	2^{25}	33554432	
8	107933601890304000	2^{24}	16777216	
9	108145236403814400	2^{23}	8388608	
10	108251053660569600	2^{22}	4194304	
11	108303962288947200	2^{21}	2097152	
12	108330416603136000	2^{20}	1048576	
13	108343643760230400	2^{19}	524288	
14	108350257338777600	2^{18}	262144	
15	108353564128051200	2^{17}	131072	
16	108355217522688000	2^{16}	65536	
17	108356044220006400	2^{15}	32768	
18	108356457568665600	2^{14}	16384	
19	108356664242995200	2^{13}	8192	
20	108356767580160000	2^{12}	4096	
21	108356819248742400	2^{11}	2048	
22	108356845083033600	2^{10}	1024	
23	108356858000179200	2^{9}	512	
24	108356864458752000	2^{8}	256	
25	108356867688038400	2^{7}	128	
26	108356869302681600	2^{6}	64	
27	108356870110003200	2^{5}	32	
28	108356870513664000	2^{4}	16	
29	108356870715494400	2^{3}	8	
30	108356870816409600	2^{2}	4	
31	108356870866867200	2^{1}	2	
32	108356870892096000	2^{0}	1	
33	108356870904710400	2^{-1}	0.5	
34	108356870911017600	2^{-2}	0.25	
35	108356870914171200	2^{-3}	0.125	
36	108356870915748000	2^{-4}	0.0625	
37	108356870916536400	2^{-5}	0.03125	
38	108356870916930600	2^{-6}	0.015625	
39	108356870917127700	2^{-7}	0.0078125	
40	108356870917226250	2^{-8}	0.00390625	
41	108356870917275525	2^{-9}	0.001953125	
42	108356870917300162	2^{-10}	0.0009765625	
43	108356870917312481	2^{-11}	0.00048828125	
44	108356870917318640	2^{-12}	0.000244140625	
45	108356870917321720	2^{-13}	0.0001220703125	
46	108356870917323260	2^{-14}	6.103515625e-05	
47	108356870917324030	2^{-15}	3.0517578125e-05	
48	108356870917324415	2^{-16}	1.52587890625e-05	
49	108356870917324607	2^{-17}	7.62939453125e-06	
50	108356870917324703	2^{-18}	3.814697265625e-06	
51	108356870917324751	2^{-19}	1.9073486328125e-06	
52	108356870917324775	2^{-20}	9.5367431640625e-07	
53	108356870917324787	2^{-21}	4.76837158203125e-07	
54	108356870917324793	2^{-22}	2.384185791015625e-07	
55	108356870917324796	2^{-23}	1.1920928955078125e-07	
56	108356870917324798	2^{-24}	5.9604644775390625e-08	
57	108356870917324799	2^{-25}	2.98023223876953125e-08	
58	108356870917324799	2^{-26}	1.490116119384765625e-08	
59	108356870917324799	2^{-27}	7.450580596923828125e-09	
60	108356870917324799	2^{-28}	3.7252902984619140625e-09	
61	108356870917324799	2^{-29}	1.86264514923095703125e-09	
62	108356870917324799	2^{-30}	9.31322574615478515625e-10	
63	108356870917324799	2^{-31}	4.656612873077392578125e-10	
64	108356870917324799	2^{-32}	2.3283064365386962890625e-10
```

### max_moneyBTC (optional)
<!-- ![](https://github.com/sugarchain-project/yumekawa-utils/blob/master/max_moneyBTC/max_moneyBTC.png) -->

 - data BTC
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