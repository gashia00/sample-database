# [<img src="https://ipinfo.io/static/ipinfo-small.svg" alt="IPinfo" width="24"/>](https://ipinfo.io/) IPinfo Sample Database Repository


## Sample datasets of all the [IP address database products](https://ipinfo.io/account/data-downloads).


<p align="center">
  <img src="./assets/header_grahics_main_readme.png">
</p>

<!-- TOC: Manually Generated -->
- [Database Overview](#database-overview)
- [Features of the Repository](#features-of-the-repository)
- [Summary of the Databases](#summary-of-the-databases)
    - [IP to Country](#ip-to-country)
    - [IP to ASN](#ip-to-asn)
    - [IP to Country + ASN](#ip-to-country--asn)
    - [IP Geolocation](#ip-geolocation)
    - [IP to Company](#ip-to-company)
    - [ASN Database](#asn-database)
    - [IP to Mobile Carrier](#ip-to-mobile-carrier)
    - [Privacy Detection](#privacy-detection--anonymous-ip-detection)
    - [Hosted Domains](#hosted-domains--reverse-ip-lookup)
    - [Abuse Contact](#abuse-contact)
    - [IP Geolocation Extended](#ip-geolocation-extended)
    - [Privacy Detection Extended](#privacy-detection-extended)
    - [WHOIS](#whois)
- [Relevant Articles](#relevant-articles)
  - [Guides](#guides)
  - [FAQs](#faqs)
- [About IPinfo](#about-ipinfo)

# Database Overview

<p align="center">
  <img src="./assets/product_demo_main_readme.gif">
</p>

The database products [IPinfo.io](https://ipinfo.io) has to offer are -

| Database Product | Sample Database Repo | Description |
| --- | --- | --- |
| [IP Geolocation Database](https://ipinfo.io/products/ip-geolocation-database) | [IP Geolocation Sample](/IP%20Geolocation) | IP geolocation information |
| [IP to Company Database](https://ipinfo.io/products/ip-company-database) | [IP to Company Sample](/IP%20to%20Company) | Company associated with IP address |
| [ASN Database](https://ipinfo.io/products/asn-database) | [ASN Database Sample](/ASN%20Database) | IP range and ASN information |
| [IP to Mobile Carrier Database](https://ipinfo.io/products/mobile-ip-database) | [IP to Mobile Sample](/IP%20to%20Mobile%20Carrier) | Mobile carrier and country information |
| [Privacy Detection Database](https://ipinfo.io/products/anonymous-ip-database) | [Privacy Detection Sample](/Privacy%20Detection) | VPN, proxy, Tor, relay detection |
| [Hosted Domain Database](https://ipinfo.io/products/hosted-domains-database) | [Hosted Domains Sample](/Hosted%20Domains) | Reverse IP lookup |
| [Abuse Contact Database](https://ipinfo.io/products/ip-abuse-contact-database) | [Abuse Contact Sample](/Abuse%20Contact) | Abuse contact information |
| [WHOIS Database](https://ipinfo.io/products/ip-whois-data-download) | [WHOIS Sample](/WHOIS) | Contextualized and structured WHOIS database |


IPinfo also provides the following [IP databases for free](https://ipinfo.io/products/free-ip-database). The database provide full accuracy, daily updates and complete IP data solution. The databases are licensed under (CC BY-SA 4.0) and require an attribution statement, which can found on your account dashboard.

| Database Product | Sample Database Repo | Description |
| --- | --- | --- |
| [IP to Country](https://ipinfo.io/products/free-ip-database) | [IP to Country Sample](/IP%20to%20Country) | IP to Country Information|
| [IP to ASN](https://ipinfo.io/products/free-ip-database) | [IP to ASN Sample](/IP%20to%20ASN) | IP to ASN information |
| [IP to Country + ASN](https://ipinfo.io/products/free-ip-database) | [IP to Country + ASN Sample](/IP%20to%20Country%20ASN) | Joined database of IP to Country and IP to ASN|

We offer a few detailed database that comes with additional columns that gives insights to the accuracy and our data methodology. These enterprise grade databases are only available upon request.

| Database Product | Sample Database Repo | Description
| --- | --- | --- |
| IP to Geolocation Extended Database | [IP to Geolocation Extended Sample](/IP%20Geolocation%20Extended) | IP to Geolocation database with accuracy radius
| IP to Privacy Detection Extended Database | [IP to Privacy Detection Extended Sample](/Privacy%20Detection%20Extended) | IP to Privacy Detection database detection method information


**All of these products are available as CSV, JSON and MMDB type.**

# Features of the Repository

Please visit each folder to learn more about the databases. Each directory README contains -

- Sample Dataset (100 rows) in `.csv`, `.json` and `.mmdb` format
- API response (in `.json`)
- Breakdown of the dataset with description of the fields
- Breakdown of the API response
- Helpful guides, resources and articles


# Summary of the Databases

Please visit the individual database directories to learn more. The database schemas were generated in February, 2023.

<details id=1>
<summary><h2>IP to Country</h2></summary>

**Get the country and continent information from IP addresses.**

You can find the schema, database sample, API response sample, and other information in the **[IP to Country folder](/IP%20to%20Country)**. The database includes the following fields:

| Field Name       | Example         | Description                                |
|------------------|-----------------|--------------------------------------------|
| `start_ip`       | 217.220.0.0     | Starting IP address of an IP address range |
| `end_ip`         | 217.223.255.255 | Ending IP address of an IP address range   |
| `country`        | IT              | ISO 3166 country code of the location      |
| `country_name`   | Italy           | Name of the country                        |
| `continent`      | EU              | Continent code of the country              |
| `continent_name` | Europe          | Name of the continent                      |


</details>

<details id=2>
<summary><h2>IP to ASN</h2></summary>

**Get ASN information (limited) from an IP address range.**

You can find the schema, database sample, API response sample, and other information in the **[IP to ASN folder](/IP%20to%20ASN)**. The database includes the following fields:

| Field Name | Example       | Description                                       |
|------------|---------------|---------------------------------------------------|
| `start_ip` | 62.235.50.0   | Starting IP address of an IP address range        |
| `end_ip`   | 62.235.50.255 | Ending IP address of an IP address range          |
| `asn`      | AS29005       | Autonomous System Number                          |
| `name`     | Proximus NV   | Name of the AS (Autonomous System) organization   |
| `domain`   | proximus.com  | Official domain or website of the AS organization |


</details>


<details id=3>
<summary><h2>IP to Country + ASN</h2></summary>

**Joined database of IP to Country and IP to ASN database.**

You can find the schema, database sample, API response sample, and other information in the **[IP to Country ASN folder](/IP%20to%20Country%20ASN)**. The database includes the following fields:

| Field Name       | Example        | Description                                       |
|------------------|----------------|---------------------------------------------------|
| `start_ip`       | 194.87.139.0   | Starting IP address of an IP address range        |
| `end_ip`         | 194.87.139.255 | Ending IP address of an IP address range          |
| `country`        | NL             | ISO 3166 country code of the location             |
| `country_name`   | Netherlands    | Name of the country                               |
| `continent`      | EU             | Continent code of the country                     |
| `continent_name` | Europe         | Name of the continent                             |
| `asn`            | AS1239         | Autonomous System Number                          |
| `as_name`        | Sprint         | Name of the AS (Autonomous System) organization   |
| `as_domain`      | sprint.net     | Official domain or website of the AS organization |


</details>

<details id=4>
<summary><h2>IP Geolocation</h2></summary>

**Get geolocation information from IP addresses.**

You can find the schema, database sample, API response sample, and other information in the **[IP Geolocation folder](/IP%20Geolocation)**. The database includes the following fields:

| Field Name    | Example          | Description                                     |
|---------------|------------------|-------------------------------------------------|
| `start_ip`    | 1.253.242.0      | Starting IP address of an IP address range      |
| `end_ip`      | 1.253.242.255    | Ending IP address of an IP address range        |
| `join_key`    | 1.253.0.0        | Special variable to facilitate `join` operation |
| `city`        | Yangsan          | City of the location                            |
| `region`      | Gyeongsangnam-do | Region of the location                          |
| `country`     | KR               | ISO 3166 country code of the location           |
| `latitude`    | 35.34199         | Latitude value of the location                  |
| `longitude`   | 129.03358        | Longitude value of the location                 |
| `postal_code` | 50593            | Postal code of the location                     |
| `timezone`    | Asia/Seoul       | Local time zone                                 |



### 🔗 [IP Geolocation Database Product Page](https://ipinfo.io/products/ip-geolocation-database)

</details>

<details id=5>
<summary><h2>IP to Company</h2></summary>

**Get firmographics data and identify the company behind the IP address and network traffic.**

You can find the schema, database sample, API response sample, and other information in the **[IP to Company folder](/IP%20to%20Company)**. This database is can be used to identify large scale organization or companies behind IP address ranges. The database includes the following fields:

| Field Name  | Example                 | Description                                                |
|-------------|-------------------------|------------------------------------------------------------|
| `start_ip`  | 107.136.106.168         | Starting IP address of an IP address range                 |
| `end_ip`    | 107.136.106.175         | Ending IP address of an IP address range                   |
| `join_key`  | 107.136.0.0             | Specialized variable to facilitate `join` operation        |
| `name`      | ZSPEC FLOW-180709174314 | Name of the company                                        |
| `domain`    | zspec.com               | Domain of the company                                      |
| `type`      | business                | Type of business. e.g. Business, ISP, Hosting or Education |
| `asn`       | AS7018                  | ASN associated with the company                            |
| `as_name`   | AT&T Services, Inc.     | Name of the ASN                                            |
| `as_domain` | att.com                 | Domain name of the ASN                                     |
| `as_type`   | isp                     | ASN Type: ISP, Hosting, Business or Education              |
| `country`   | US                      | ISO 3166 country code                                      |



### 🔗 [IP to Company Database Product Page](https://ipinfo.io/products/ip-company-database)

</details>

<details id=6>
<summary><h2>ASN Database</h2></summary>


**Get ASN data from ASN or IP Address information.**

You can find the schema, database sample, API response sample, and other information in the **[ASN folder](/ASN%20Database)**. The Database contains the following fields:

| Field Name | Example             | Description                                     |
|------------|---------------------|-------------------------------------------------|
| `start_ip` | 125.113.0.0         | Starting IP address of the ASN IP address block |
| `end_ip`   | 125.113.255.255     | Ending IP address of the ASN IP address block   |
| `join_key` | 125.113.0.0         | Special variable to facilitate `join` operation |
| `asn`      | AS4134              | Autonomous System Number (ASN)                  |
| `domain`   | chinatelecom.com.cn | Domain name of the AS                           |
| `name`     | CHINANET-BACKBONE   | Name of the ASN                                 |
| `type`     | isp                 | ASN Type: ISP, Hosting, Education or Business   |
| `country`  | CN                  | ISO 3166 country code                           |


### 🔗 [ASN Database Product Page](https://ipinfo.io/products/asn-database)

</details>

<details id=7>
<summary><h2>IP to Mobile Carrier</h2></summary>

**Lookup Mobile Carrier data such as - MCC and MNC from IP addresses.** 

You can find the schema, database sample, API response sample, and other information in the **[IP to Mobile Carrier folder](/IP%20to%20Mobile%20Carrier)**. The database contains the following fields:

| Field Name | Example                                  | Description                                      |
|------------|------------------------------------------|--------------------------------------------------|
| `start_ip` | 5.208.203.0                              | Starting IP address of an IP address range       |
| `end_ip`   | 5.208.203.255                            | Ending IP address of an IP address range         |
| `join_key` | 5.208.0.0                                | Special variable to facilitate `join` operation. |
| `name`     | Mobile Communication Company of Iran PLC | Name of the mobile carrier                       |
| `country`  | IR                                       | ISO 3166 country code                            |
| `mcc`      | 432                                      | Mobile Country Code (MCC) of the carrier         |
| `mnc`      | 11                                       | Mobile Network Code (MNC) of the carrier         |


### 🔗 [IP to Mobile Carrier Database Product Page](https://ipinfo.io/products/mobile-ip-database)

</details>

<details id=8>
<summary><h2>Privacy Detection / Anonymous IP Detection</h2></summary>

**Demystify anonymous IP addresses. Identify privacy masking services such as VPN, Tor, proxies, relays and hosting from IP addresses.**

You can find the schema, database sample, API response sample, and other information in the **[Privacy Detection folder](/Privacy%20Detection)**. The database includes the following fields:

| Field Name | Example     | Description                                                                                                                  |
|------------|-------------|------------------------------------------------------------------------------------------------------------------------------|
| `start_ip` | 115.9.76.79 | Starting IP address of an IP address range                                                                                   |
| `end_ip`   | 115.9.76.79 | Ending IP address of an IP address range                                                                                     |
| `join_key` | 115.9.0.0   | Special variable to facilitate `join` operation                                                                              |
| `hosting`  |             | Indicates a hosting IP address most of the time based on a data center. Indicative of bots, scrapers or malicious activities |
| `proxy`    |             | Similar to VPN mainly used by businesses                                                                                     |
| `tor`      |             | IP address originated from the Onion router                                                                                  |
| `vpn`      | True        | Virtual Private Network (VPN) service IP address                                                                             |
| `relay`    |             | Traffic relays often provided by CDN companies                                                                               |
| `service`  |             | Name of the privacy service provider                                                                                         |



### 🔗 [Privacy Detection Database Product Page](https://ipinfo.io/products/anonymous-ip-database)

</details>

<details id=9>
<summary><h2>Hosted Domains / Reverse IP Lookup</h2></summary>

**Hosted Domains database enables you to do reverse IP lookups.**

Through our Hosted Domains service, you can see the full list of domains hosted on a single IP address. 

You can find the schema, database sample, API response sample, and other information in the **[Hosted Domains folder](/Hosted%20Domains)**. The database includes the following fields:

| Field Name | Example                                  | Description                                    |
|------------|------------------------------------------|------------------------------------------------|
| `ip`       | 135.125.236.225                          | IP address for reverse IP lookup               |
| `total`    | 3                                        | Number of domains registered to the IP Address |
| `domains`  | farmanaut.com,pharmanaut.be,farmanaut.be | Name of the domain(s) under the IP address     |


### 🔗 [Hosted Domains Database Product Page](https://ipinfo.io/products/hosted-domains-database)

</details>

<details id=10>
<summary><h2>Abuse Contact</h2></summary>

**Get the abuse contact information of every ISP on the internet.**

You can find the schema, database sample, API response sample, and other information in the **[Abuse Contact folder](/Abuse%20Contact)**. The database includes the following fields:

| Field Name | Example                                           | Description                                      |
|------------|---------------------------------------------------|--------------------------------------------------|
| `start_ip` | 119.93.20.248                                     | Starting IP address of an IP address block       |
| `end_ip`   | 119.93.20.255                                     | Ending IP address of an IP address block         |
| `join_key` | 119.93.0.0                                        | Special variable to facilitate `join` operation  |
| `name`     | Nilo Agir                                         | Name of the abuse contact                        |
| `email`    | abuse@pldt.net                                    | Organizational email of the abuse contact        |
| `address`  | Philippine Long Distance Telephone Company, 6/... | Organizational address of the abuse contact      |
| `country`  | PH                                                | ISO 3166 country code                            |
| `phone`    | +632-584-1045                                     | Organizational phone number of the abuse contact |


### 🔗 [Abuse Contact Database Product Page](https://ipinfo.io/products/ip-abuse-contact-database)

</details>

<details id=11>
<summary><h2>IP Geolocation Extended</h2></summary>

**IP to Geolocation database with confidence metric or accuracy radius for each entry**

You can find the schema, database sample, API response sample, and other information in the **[IP Geolocation Extended folder](/IP%20Geolocation%20Extended)**. The database includes the following fields:

| Field Name    | Example             | Description                                                  |
|---------------|---------------------|--------------------------------------------------------------|
| `start_ip`    | 171.71.0.0          | Starting IP address of an IP address range                   |
| `end_ip`      | 171.71.127.255      | Ending IP address of an IP address range                     |
| `join_key`    | 171.71.0.0          | Special variable to facilitate `join` operation              |
| `city`        | San Jose            | City of the location                                         |
| `region`      | California          | Region of the location                                       |
| `country`     | US                  | ISO 3166 country code of the location                        |
| `latitude`    | 37.4087             | Latitude value of the location                               |
| `longitude`   | -121.9406           | Longitude value of the location                              |
| `postal_code` | 95134               | Postal code of the location                                  |
| `timezone`    | America/Los_Angeles | Local time zone                                              |
| `geoname_id`  | 5392171             | `Geonames_id` from [geonames.org](https://www.geonames.org/) |
| `radius`      | 5                   | Accuracy radius in terms of kilometers                       |



</details>


<details id=12>
<summary><h2>Privacy Detection Extended</h2></summary>

**Get detection method for each private IP address**

You can find the schema, database sample, API response sample, and other information in the **[Privacy Detection Extended folder](/Privacy%20Detection%20Extended)**. The database includes the following fields:

| Fields            | Example       | Description                                                                                                                          |
|-------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------|
| `start_ip`        | 62.182.99.0   | First IP address of the range                                                                                                        |
| `end_ip`          | 62.182.99.255 | Last IP address of the range                                                                                                         |
| `join_key`        | 62.182.0.0    | Specialized variable to facilitate join operation                                                                                    |
| `hosting`         | False         | Indicates hosting service IP address (data center, cloud service, bots, scrapers,  etc.)                                             |
| `proxy`           | False         | IP address associated with a proxy service                                                                                           |
| `tor`             | False         | Tor exit node IP address                                                                                                             |
| `vpn`             | True          | IP address associated with a VPN service                                                                                             |
| `relay`           | False         | Private relay service IP address (Apple relay, Cloudflare, Akamai etc.)                                                              |
| `vpn_name`        | NordVPN       | Name of the privacy service provider includes VPN, Proxy and Relay service providers names                                           |
| `anycast`         | False         | True: if IP is indentified as being any anycast IP, that could map to multiple physical servers in different locations               |
| `census`          | True          | True: if we've indentified VPN software running on this IP as part of our internet wide scan (successful openvpn or ipsec handshake) |
| `device_activity` | True          | True: if we've seen VPN-like behavior (multiple devices, multiple locations etc)                                                     |
| `whois`           | False         | True: if we've seen vpn provider attributes in the IP whois data (eg. provider name)                                                 |
| `vpn_config`      | True          | True: if we've identified this IP in a VPN config file                                                                               |
| `census_port`     | 500           | Port number we've identified VPN software running on                                                                                 |

</details>

<details id=13>
<summary><h2>WHOIS</h2></summary>


**IPinfo WHOIS database is a contextual, robust and consistent database of various types of WHOIS data.**

You can find the schema, database sample, API response sample, and other information in the **[WHOIS folder](/WHOIS)**. The WHOIS database and their respective fields are listed below:

### R WHOIS

| Field Name | Example | Description |
| --- | --- | --- |
| `range` | 50.28.18.195 | IP Address range/netblock |
| `id` | NETBLK-GRADOCEROPUB.50.28.18.195/32 | Raw netblock identifier from WHOIS |
| `name` | Grado Cero Publicidad S.A. de C.V. | Name of netblock |
| `descr` | GRADOCEROPUB-50.28.18.195 | Description |
| `host` | rwhois.liquidweb.com:4321 | Host information |
| `country` | MX | ISO 3166 country code |
| `email` | webmaster@gradocero.com | Contact email information |
| `abuse` | abuse@sourcedns.com | Abuse email information |
| `domain` | gradocero.com | Domain associated with the netblock |
| `country.1` | MX | Secondary country information |
| `city` | Naucalpan de Juarez | City information |
| `street` | Calle Andes #46 | Street information |
| `postal` | 53125 | Postal Code information |
| `updated` | 2021-01-26 00:00:00 | Update date in the WHOIS registry |
| `imported` | 2021-01-27 04:44:47.206483 | Imported date in the WHOIS registry |


### RIR WHOIS

| Field Name | Example | Description |
| --- | --- | --- |
| `range` | 45.142.160.224-45.142.161.255 | IP Address range/netblock |
| `id` | PL-DOMYNET-NETWORK | Raw netblock identifier from WHOIS |
| `name` | DomyNet Sp. z o.o. | Name of netblock |
| `country` | PL | ISO 3166 country code |
| `status` | ASSIGNED PA | Range assignment type ([RIPE’s documentation](https://www.ripe.net/publications/docs/ripe-733)) |
| `tech` | PK9274-RIPE | ID for technical contact of WHOIS record |
| `maintainer` | MNT-PL-DOMYNET-1 | ID for contact authorized to update WHOIS record for netblock |
| `admin` | PK9274-RIPE | ID for administrative contact of netblock |
| `source` | ripe | RIR associated with record (RIPE, ARIN, etc.) |
| `whois_domain` | domynet.pl | Domain name (from WHOIS entry) |
| `updated` | 2020-01-09 | Last updated date (taken from WHOIS entry) |
| `org` | ORG-DSZO39-RIPE | ID or name of organization responsible for netblock |
| `rdns_domain` | domynet.pl | Domain associated with IP range (only available if a majority of IPs within range share a common reverse DNS domain) |
| `domain` | domynet.pl | Domain associated with netblock (based on our data sets) |
| `geoloc` | 52.2260524 20.9941955 | Latitude/longitude coordinates indicating where users of network are located |
| `org_address` | ul. Lindleya 16/301 02-013 Warszawa POLAND | Address of the associated organization |
| `asn` | AS208348 | Autonomous system number for organization that routes traffic for IP (based on BGP routing data) |
| `as_name` | DomyNet Sp. z o.o. | Name of AS (based on our data sets and data processing) |
| `as_domain` | domynet.pl | Domain of AS (based on our data sets and data processing) |
| `as_type` | isp | ISP, business, or hosting (based on around 20 different features and our custom training set) |


<details id=14>
<summary><h3>Other WHOIS Databases</h3></summary>

Other kinds of WHOIS Database IPinfo offers:

| WHOIS ASN | WHOIS MNT | WHOIS NET | WHOIS ORG | WHOIS POC |
| --- | --- | --- | --- | --- |
| id | id | range | id | id |
| name | name | id | name | name |
| country | admin_id | name | address | mobilephone |
| org_id | tech_id | country | street | officephone |
| created | org_id | domain | city | fax |
| updated | created | org_id | state | addres |
| source | updated | status | postalcode | country |
| raw | source | tech_id | country | email |
|  | raw | mnt_id | admin_id | abuse_email |
|  |  | admin_id | tech_id | created |
|  |  | created | abuse_id | updated |
|  |  | updated | mnt_id | source |
|  |  | source | email | raw |
|  |  | raw | domain |  |
|  |  |  | created |  |
|  |  |  | updated |  |
|  |  |  | source |  |
|  |  |  | raw |  |

</details>

### 🔗 [WHOIS Database Product Page](https://ipinfo.io/products/ip-whois-data-download)

</details>

# Other Information (Usage, Exploration etc.)

**How to explore the sample databases**

- Please visit the folders for each database. You can also find the API response samples there for each product.
- If you would like to explore CSV files, feel free to use any of these online services and import the raw CSV there -
    - [DuckDB] [CSVfiddle](https://csvfiddle.io/)
    - [SQLite3] [Datasette](https://lite.datasette.io/)
    - [PostgreSQL] [Bit.io](https://bit.io/)
- Or you can you just download the CSV files to take a closer look.
- You can also check out `.mmdb` sample files. Please use IPinfo's [mmdbctl](https://github.com/ipinfo/mmdbctl) tool to explore them.

**Usage Information**

- After signing up for database downloads service, you can either download the database from our website or you can `curl` the database from the database download endpoint. But make sure you have redirect [enabled](https://ipinfo.io/faq/article/142-when-i-access-the-database-endpoint-using-something-like-curl-it-doesn-t-seem-to-work-and-i-get-a-corrupted-empty-file-what-am-i-doing-wrong).
- You can select how frequently the database gets updated. It can be daily, weekly, bi-weekly or monthly.
- To look up an specific database, you can use any kind of data exploration package or database system you want to use. [Here is an example](https://ipinfo.io/faq/article/144-how-do-you-do-a-lookup-of-an-ip-address-using-your-database) of using MySQL and PostgreSQL to look up a specific IP address.

# Relevant Articles

## Guides

- [How to choose the best file format for your IPinfo database?](https://ipinfo.io/blog/ipinfo-database-formats/)
- [How to get IP data and IP location in C# with IPinfo](https://ipinfo.io/blog/ip-geolocation-c-sharp/)
- [Our downloadable IP WHOIS data sets are live!](https://ipinfo.io/blog/our-downloadable-ip-whois-data-sets-are-live)
- [Data downloads vs API, or both?](https://ipinfo.io/blog/data-downloads-vs-api-or-both/)
- [Ingesting IPinfo geolocation data with PostgreSQL 13](https://ipinfo.io/blog/ingesting-ipinfo-geolocation-data-with-postgresql-13/)
- [Introducing a Simpler Way to get IP Address Data in Snowflake](https://ipinfo.io/blog/ip-address-data-in-snowflake/)
- [IP data enrichment with IPinfo: 4 ways to add insights to your traffic/server logs](https://ipinfo.io/blog/ip-data-enrichment-in-4-ways/)
- [Meet IPinfo’s Free IP Data Downloads](https://ipinfo.io/blog/meet-free-ip-address-database/)

## FAQs

The list of FAQs (Frequently Asked Questions) can be found [here](https://ipinfo.io/faq/category/137-data-downloads).

# Found a bug?

If you found an issue or would like to submit an improvement to this project, please submit an issue using the issues tab above. If you would like to submit a PR with a fix, reference the issue you created!

# Interested in more?

Currently, we are limiting the sample datasets to only **100 rows**. If you would like to request a larger sample or would like to get a quote on the database products, **[feel free to reach to us](https://ipinfo.io/products/ip-database-download#request_form)**.

Follow us on [Twitter](https://twitter.com/ipinfoio) and [LinkedIn](https://www.linkedin.com/company/ipinfo/) to learn more about IP Address data and it’s fascinating potential.

---

# IPinfo Tools

There are official IPinfo client libraries available for many languages including PHP, Python, Go, Java, Ruby, and many popular frameworks such as Django, Rails and Laravel. There are also many third party libraries and integrations available for our API.

We also have an excellent CLI tool (**930 Stars on Github**) and mapping tool.

See [https://ipinfo.io/developers/libraries](https://ipinfo.io/developers/libraries) for more details.

# About IPinfo

Founded in 2013, IPinfo prides itself on being the most reliable, accurate, and in-depth source of IP address data available anywhere. We process terabytes of data to produce our custom IP geolocation, company, carrier, VPN detection, hosted domains, and IP type data sets. Our API handles over 40 billion requests a month for 100,000 businesses and developers.

[![image](https://avatars3.githubusercontent.com/u/15721521?s=128&u=7bb7dde5c4991335fb234e68a30971944abc6bf3&v=4)](https://ipinfo.io/)