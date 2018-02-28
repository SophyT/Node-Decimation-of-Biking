# Node-Decimation-of-Biking
Python codes for simplifying routes based on Douglas-Peucker algorithm

During my internship in this winter vocation, I mainly deal with data analysis, data processing and data mining of shared bikes and subways. Position and corresponding time of using bikes are recorded a few times in one second. Therefore, massive journey data is produced and they are too memory-consuming and time-consuming for further analysis and processing.  One of my tasks is to simplify these journey data. 

I was given CSV file in two forms. 

For the Form1 CSV file
orderid,userid,bikeid,starttime,startpositionx,startpositiony,endtime,endpositionx,endpositiony===track  
1,36055029,26628,2017-06-23 20:38:05.0,114.42216905,30.60583035,2017-06-23 20:48:10.0,117.26309436,34.81314581   
6,21892173,87331,2017-06-19 20:36:06.0,116.34319661,39.99151340,2017-06-19 20:42:15.0,116.35146041,39.99155921===#116.343378,39.991452;1497875775457#116.343341,39.991487;1497875776720#116.343327,39.991476;1497875778114#116.343362,39.991422;1497875820127#116.343372,39.991360;1497875823148#116.343392,39.991316;1497875826151#116.343404,39.991260;1497875830149#116.343398,39.991214;1497875832146#116.343398,39.991152;1497875835304#116.343398,39.991152;1497875836066#116.343393,39.991085;1497875838143#116.343409,39.991019;1497875841144#116.343467,39.990983;1497875843146#116.343541,39.990961;1497875845155#116.343606,39.990960;1497875847142#116.343669,39.990962;1497875849151#116.343734,39.990961;1497875851142#116.343796,39.990963;1497875853173#116.343858,39.990955;1497875856153#116.343915,39.990943;1497875859155#116.343975,39.990920;1497875862155#116.344048,39.990924;1497875865153#116.344128,39.990924;1497875868158#116.344206,39.990913;1497875871162#116.344290,39.990924;1497875874158#116.344368,39.990932;1497875877149

Above are two orders(I have altered values)

To process Form1 file, first use ConvertComma.csv to convert the file into a new one that is easier to be processed and then to use process_form1.py to process data.

For the Form2 CSV file
Orderid,Userid,Bikeid,Time,Lng,Lat  
1274,82151654,1483949,30216,114.28215034,30.587905  
1274,82151654,1483949,30845,114.28906762,30.58603047  
1274,82151654,1483949,30870,114.289147,30.584945

Above is one order(I have altered values).
To process Form2 file, use process_form2.py.
