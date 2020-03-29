# Hotel Bookings
## Overview
In this dataset, we will be analyzing two hotels that are located in Portugal.  One is a resort hotel located in the region of Algarve and the other is a city hotel located in the city of Lisbon.  We want to predict whether some one will cancel a booking based on the data that we have.  For more information about this dataset, please read the article [Hotel booking demands dataset](https://www.sciencedirect.com/science/article/pii/S2352340918315191?via%3Dihub).

## Dataset
|Variable |Class |Description|
|---------|------|-----------|
| hotel | character | Hotel (H1 = Resort Hotel or H2 = City Hotel) |
| is_canceled | double | Value indicating if the booking was canceled (1) or not (0) |
| lead_time | double | Number of days that elapsed between the entering date of the booking into the PMS and the arrival date |
| arrival_date_year | double | Year of arrival date |
| arrival_date_month | double | Month of arrival date |
| arrival_date_week_number	 | double | Week number of year for arrival date |
| arrival_date_day_of_month | character | Day of arrival date |
| stays_in_weekend_nights | double | Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel |
| stays_in_week_nights | double | Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel |
| adults | double | Number of adults |
| children | double | Number of children |
| babies | double | Number of babies |
| meal | character | Type of meal booked. Categories are presented in standard hospitality meal packages: <br/> Undefined/SC – no meal package; <br/> BB – Bed & Breakfast; <br/> HB – Half board (breakfast and one other meal – usually dinner); <br/> FB – Full board (breakfast, lunch and dinner) |
| country | character | Country of origin. Categories are represented in the ISO 3155–3:2013 format.  See next table for details |
| market_segment | character | Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators” |
| distribution_channel | character | Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators” |
| is_repeated_guest | double | Value indicating if the booking name was from a repeated guest (1) or not (0) |
| previous_cancellations | double | Number of previous bookings that were cancelled by the customer prior to the current booking |
| previous_bookings_not_canceled | double | Number of previous bookings not cancelled by the customer prior to the current booking |
| reserved_room_type | character | Code of room type reserved. Code is presented instead of designation for anonymity reasons |
| assigned_room_type | character | Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons |
| booking_changes | double | Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation |
| deposit_type | character | Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories: <br/> No Deposit – no deposit was made; <br/> Non Refund – a deposit was made in the value of the total stay cost; <br/> Refundable – a deposit was made with a value under the total cost of stay. |
| agent | character | ID of the travel agency that made the booking |
| company | character | ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons |
| days_in_waiting_list | double | Number of days the booking was in the waiting list before it was confirmed to the customer |
| customer_type | character | Type of booking, assuming one of four categories: <br/> Contract - when the booking has an allotment or other type of contract associated to it; <br/> Group – when the booking is associated to a group; <br/> Transient – when the booking is not part of a group or contract, and is not associated to other transient booking; <br/> Transient-party – when the booking is transient, but is associated to at least other transient booking |
| adr | double | Average Daily Rate as defined by dividing the sum of all lodging transactions by the total number of staying nights |
| required_car_parking_spaces	 | double | Number of car parking spaces required by the customer |
| total_of_special_requests | double | Number of special requests made by the customer (e.g. twin bed or high floor) |
| reservation_status | character | Reservation last status, assuming one of three categories: <br/> Canceled – booking was canceled by the customer; <br/> Check-Out – customer has checked in but already departed; <br/> No-Show – customer did not check-in and did inform the hotel of the reason why |
| reservation_status_date	 | double | Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel |

### Country Details
|Country Code| Country|
|------------|--------|
PRT|	Portugal
GBR|	Great Britain
USA|	United States
ESP|	Spain
IRL|	Ireland
FRA|	France	
ROU|	Romania
NOR|	Norway
OMN|	Oman
ARG|	Argentina
POL|	Poland
DEU|	Germany
BEL|	Belgium
CHE|	Switzerland
CN|	China
GRC|	Greece
ITA|	Italy
NLD|	the Netherlands
DNK|	Denmark
RUS|	Russia
SWE|	Sweden
AUS|	Australia
EST|	Estonia
CZE|	Czechia
BRA| Brazil
FIN| Finland
MOZ|	Mozambique
BWA|	Botswana
LUX|	Luxembourg
SVN|	Slovenia
ALB|	Albania
IND|	India
CHN|	China
MEX|	Mexico
MAR|	Morocco
UKR|	Ukraine
SMR|	San Marino
LVA|	Latvia
PRI|	Puerto Rico
SRB|	Serbia
CHL|	Chile
AUT|	Austria
BLR|	Belarus
LTU|	Lithuania
TUR|	Turkey
ZAF|	South Africa
AGO|	Angola
ISR|	Israel
CYM|	Cayman Islands
ZMB|	Zambia
CPV|	Cabo Verde
ZWE|	Zimbabwe
DZA|	Algeria
KOR|	Korea
CRI|	Costa Rica
HUN|	Hungary
ARE|	United Arab Emirates
TUN|	Tunisia
JAM|	Jamaica
HRV|	Croatia
HKG|	Hong Kong
IRN|	Iran
GEO|	Georgia
AND|	Andorra
GIB|	Gibraltar
URY|	Uruguay
JEY|	Jersey
CAF|	Central African Republic
CYP|	Cyprus
COL|	Colombia
GGY|	Guernsey
KWT|	Kuwait
NGA|	Nigeria
MDV|	Maldives
VEN|	Venezuela
SVK|	Slovakia
FJI|	Fiji
KAZ|	Kazakhstan
PAK|	Pakistan
IDN|	Indonesia
LBN|	Lebanon
PHL|	Philippines
SEN|	Senegal
SYC|	Seychelles
AZE|	Azerbaijan
BHR|	Bahrain
NZL|	New Zealand
THA|	Thailand
DOM|	Dominican Republic
MKD|	North Macedonia
MYS|	Malaysia
ARM|	Armenia
JPN|	Japan
LKA|	Sri Lanka
CUB|	Cuba
CMR|	Cameroon
BIH|	Bosnia and Herzegovina
MUS|	Mauritius
COM|	Comoros
SUR|	Suriname
UGA|	Uganda
BGR|	Bulgaria
CIV|	Cote d'Ivoire
JOR|	Jordan
SYR|	Syrian Arab Republic
SGP|	Singapore
BDI|	Burundi
SAU|	Saudi Arabia
VNM|	Viet Nam
PLW|	Palau
QAT|	Qatar
EGY|	Egypt
PER|	Peru
MLT|	Malta
MWI|	Malawi
ECU|	Ecuador
MDG|	Madagascar
ISL|	Iceland
UZB|	Uzbekistan
NPL|	Nepal
BHS|	Bahamas
MAC|	Macao
TGO|	Togo
TWN|	Taiwan
DJI|	Djibouti
STP|	Sao Tome and Principe
KNA|	Saint Kitts and Nevis
ETH|	Ethiopia
IRQ|	Iraq
HND|	Honduras
RWA|	Rwanda
KHM|	Cambodia
MCO|	Monaco
BGD|	Bangladesh
IMN|	Isle of Man
TJK|	Tajikistan
NIC|	Nicaragua
BEN|	Benin
VGB|	Virgin Islands (British)
TZA|	Tanzania
GAB|	Gabon
GHA|	Ghana
TMP|	East Timor
GLP|	Guadeloupe
KEN|	Kenya
LIE|	Liechtenstein
GNB|	Guinea-Bissau
MNE|	Montenegro
UMI|	United States Minor Outlying
MYT|	Mayotte
FRO|	Faroe Islands
MMR|	Myanmar
PAN|	Panama
BFA|	Burkina Faso
LBY|	Libya
MLI|	Mali
NAM|	Namibia
BOL|	Bolivia
PRY|	Paraguay
BRB|	Barbados
ABW|	Aruba
AIA|	Anguilla
SLV|	El Salvador
DMA|	Dominica
PYF|	French Polynesia
GUY|	Guyana
LCA|	Saint Lucia
ATA|	Antarctica
GTM|	Guatemala
ASM|	American Samoa
MRT|	Mauritania
NCL|	New Caledonia
KIR|	Kiribati
SDN|	Sudan
ATF|	French Southern Territories
SLE|	Sierra Leone
LAO|	Lao People's Democratic Republic
