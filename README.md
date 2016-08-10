# Snort-appid
Run the Snort with Appid  
and it will creat the output named appstats-u2.xxxx  
```
$ /usr/local/bin/snort -A console -c /etc/snort/snort.conf -i eth0
```
  
#check the output file
you can use "u2openappid" to open the output in "/var/log/snort/"
```
cd /var/log/snort/
u2openappid your_output_name
```
  
#check the Mapping data of appid
```
/etc/snort/rules/odp/appMapping.data
```
  
#change the time of record
you can change the time from /etc/snort/snort.conf  
find the preprocessor appid (line 516)  
default value time is 60.  
  
#check the rule of Snort
```
/etc/snort/rules/local.rules
```
