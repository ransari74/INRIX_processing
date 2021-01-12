# Processing INRIX Data
INRIX provides user the high resolution traffic data. These data are huge in size, so, reading, cleaning, and processing it makes time. In this tutorial we provide coding to read, clean and extract data you needed from INRIX data using Pandas. However, due to the copy right law, I can not provides any sample of INRIX data in github. To download the data, INRIX provides the userfrienly UI helping customers to download data with selecting segment, corridor, or region to download data. In addition, they provides API to download files directly using query. For more information visit http://docs.inrix.com/traffic/speed/. In the following we will elaborate on the output of INRIX traffic file metadata. 

''
INRIX Roadway Analytics data downloader reports include the columns listed below.  For additional information, please visit https://analytics.inrix.com/help 
 
The attibutes INRIX provides in traffic datasets are:
 
1.Date Time	Timestamp in local time\
2.Segment ID	INRIX XD segment ID\
3.UTC Date Time	Timestamp in UTC\
4.Speed(mph or kmh)	Estimated harmonic mean speed\
5.Historic Average Speed(mph or kmh) 	Historical average speed for that hour of the day and day of the week\
6.Ref Speed(mph or kmh)	The ‘free flow speed’. The speed driven on this road when it is  wide open, based on INRIX historical data.  Note that this is not legal speed limit\
7.Travel Time (Minutes)	The travel time in minutes\
8.CValue 	The confidence value is an integer ranging from 0 to 100 inclusive that indicates the confidence that INRIX has in the correctness of a real-time speeds\
9.Pct Score30	Percentage of the segment minutes based on actual speeds data for the time period\
10.Pct Score20	Percentage of the segment minutes based on historic average speed\
11.Pct Score10	Percentage of the segment minutes based on the reference ‘free flow’ speed\
''

When you donwload data with INRIX, INRIX compresses several Segment in each Zip file. In each Zip file, you should find the CSV file o extract traffic data.
