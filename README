1. Run these commands to install the necessary software.
```
apt install docker
apt install docker-compose
```

2. In the directory you would like your maxscale subdirectory to be placed in, use git to clone a maxscale template of your choice.
```
git clone [repository URL]
```

3. Navigate to the maxscale subfolder within the new folder and edit the configuration file, replacing all version numbers with "latest" instead.
```
cd maxscale-docker/maxscale
nano docker-compose.yml
```

4. Deploy the maxscale docker images and verify that they're running properly.
```
docker-compose up -d
docker-compose exec maxscale maxctrl list servers
```

5. While in the maxscale/sql directory, you can execute SQL queries using this command as a template:
```
mysql -u []db username -p [db password] -h 127.0.0.1 -P [port] -e "SELECT * FROM [database name] LIMIT [maximum number of matching entries displayed];"
```

For example, these two commands may yield the following results:

```
mysql -u maxuser -pmaxpwd -h 127.0.0.1 -P 3306 -e "SELECT * FROM zipcodes_one.zipcodes_one LIMIT 6;"
```
Will give this output:
	
Zipcode	ZipCodeType	City		State	LocationType	Coord_Lat	Coord_Long	Location		Decommisioned	TaxReturnsFiled	EstimatedPopulation	TotalWages
705	STANDARD	AIBONITO	PR	PRIMARY		18.14		-66.26		NA-US-PR-AIBONITO	FALSE			
610	STANDARD	ANASCO		PR	PRIMARY		18.28		-67.14		NA-US-PR-ANASCO		FALSE						
611	PO BOX		ANGELES		PR	PRIMARY		18.28		-66.79		NA-US-PR-ANGELES	FALSE						
612	STANDARD	ARECIBO		PR	PRIMARY		18.45		-66.73		NA-US-PR-ARECIBO	FALSE						
601	STANDARD	ADJUNTAS	PR	PRIMARY		18.16		-66.72		NA-US-PR-ADJUNTAS	FALSE						
631	PO BOX		CASTANER	PR	PRIMARY		18.19		-66.82		NA-US-PR-CASTANER	FALSE						
	
And
```
mysql -u maxuser -pmaxpwd -h 127.0.0.1 -P 3306 -e "SELECT * FROM zipcodes_two.zipcodes_two LIMIT 6;"
```
will give this output:
																	
Zipcode	ZipCodeType	City		State	LocationType	Coord_Lat	Coord_Long	Location		Decommisioned	TaxReturnsFiled	EstimatedPopulation	TotalWages
42040	STANDARD	FARMINGTON	KY	PRIMARY		36.67		-88.53		NA-US-KY-FARMINGTON	FALSE		465		896			11562973
41524	STANDARD	FEDSCREEK	KY	PRIMARY		37.4		-82.24		NA-US-KY-FEDSCREEK	FALSE						
42533	STANDARD	FERGUSON	KY	PRIMARY		37.06		-84.59		NA-US-KY-FERGUSON	FALSE		429		761			9555412
40022	STANDARD	FINCHVILLE	KY	PRIMARY		38.15		-85.31		NA-US-KY-FINCHVILLE	FALSE		437		839			19909942
40023	STANDARD	FISHERVILLE	KY	PRIMARY		38.16		-85.42		NA-US-KY-FISHERVILLE	FALSE	1884		3733			113020684
41743	PO BOX		FISTY		KY	PRIMARY		37.33		-83.1		NA-US-KY-FISTY		FALSE			
