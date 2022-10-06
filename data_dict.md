col name | description | notes  
-----|-------|-------
backers_count | number of backers |   ✅
blurb | short description of the pledge |  ✅ ♻️ rename to description 
category | category the pledge belongs to, including category. Slug used as subcategory id | extract name as category and slug as category_sub and id as id_category ✅ ♻️
converted_pledged_amount | pledged amount converted to USD | ✅
country | country of pledge | ✅
created_at | date of creation (might be launched later!) | currrently unix stamp, needs transformation ✅  ♻️ change column  names
creator | name of creator | ♻️ extract id of creator ✅
currency | currency of pledge | ✅
currency_symbol | symbol of pledge currency | ❌
currency_trailing_code | True, False | no idea what that is ❌
current_currency | USD, GBP, EUR, etc...| unclear, not consistent witch currency of pledge ✅
deadline | end of pledge | ✅ ♻️ rename to date
disable_communication | False, True | ✅
friends | nan, '[]' | unclear ❌
fx_rate | | unclear ❌
goal | aim of pledge in the local currency |✅♻️ convert in USD
id | id of pledge | duplicates exist currently ✅
is_backing | | only consists of Nans and False ❌
is_starrable | is the project starrable | False, True, Nan ❌
is_starred | is the project starred by other users | False, True, but only 300 values❌
launched_at | launch date | ✅♻️ convert to date
location | location of pledgers| ✅♻️ keep name as city (e.g.Pittsford), state (e.g. "VT") 
name | name of the project | ✅
permissions | | only nans and empty lists ❌
photo | link to photo | ♻️ is photo included? ✅
pledged | amount pledged in local currency | ✅
profile | link to profile | ♻️ does a profile link exist? ✅
slug | slug name | ❌
source_url | link to kickstarter page | ❌
spotlight | after a project is succesfully funded, it gets the spotlight status. A way to update and show the project. False, True| https://help.kickstarter.com/hc/en-us/articles/115005135834-What-is-Spotlight-and-how-do-I-get-access-to-it- ✅ only for EDA, drop afterwards
staff_pick | True, False, improves visibility  | ✅
state | state of the pledge, 5 statuses | 'live', 'successful', 'failed', 'canceled', 'suspended' 
state_changed_at | date the status was last changed | linux timestamp ✅
static_usd_rate | |maybe exchange rate? ✅
urls | links to project |❌
usd_pledged | amount already pledged in USD |✅
usd_type | 'international', 'domestic', nan | maybe exchange rate type? ❌