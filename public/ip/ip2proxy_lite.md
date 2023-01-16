# 📖 ip2proxy_lite 
## ℹ️ Dataset info 
Description: `Proxy detection for IP addresses` 

Labels:`owner:upgini`   `dataset_type:public`   `dataset_source:ip`   

Search keys: `IP_RANGE_FROM` `IP_RANGE_TO` 

Row count: `2,317,954` 

## ℹ️ Features info:
|feature name|feature type|descrition|
|---|---|---|
|ip_country_code|STRING|Two-letter ISO country code derived from IP address|
|ip_region_name|STRING|Country region name derived from IP address|
|ip_city_name|STRING|City name derived from IP address|
|ip_isp|STRING|Name of internet service provider or company for IP address|
|ip_usage_type|STRING|Usage type (COM-commercial, ORG-organization, GOV-government, MIL-military, EDU-educational, LIB-library, CDN-content delivery network, ISP-fixed line ISP, MOB-mobile ISP, DCH-data center, SES-search engine spider, RSV-reserved) of IP address|
|ip_last_seen|INTEGER|Days of proxy last seen on IP address|
|ip_threat|STRING|Security threat reported for IP address|
