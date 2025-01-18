# Postcode-to-BRMA-lookup
Rmd to produce lookup up, linking unit postcodes in the UK to Broad Rental Market Areas (BRMAs). BRMAs are spatial units used for the administration of housing allowances for households in rented accommodation. Data available from Urban Big Data Centre: https://data.ubdc.ac.uk/datasets?q=%22postcode+to+Broad+Rental+Market+Area%22

Postcodes in Northern Ireland are not available as open data. The lookup adopts a somewhat ugly workaround by creating every possible postcode in the form "BTxx xxx" and associating it with the relevant BRMA. The great majority of 'postcodes' listed for Northern Ireland do not therefore exist in practice (c. 80%). Nevertheless, the lookup should still function, albeit less efficiently. This is another price to be paid for the lack of open data. 

In v2.2, I fixed a problem identified by a user, namely that West Dunbartonshire BRMA had been omitted from the list of BRMAs so that postcodes in that BRMA were misattributed to neighbouring BRMAs. The problem stemmed from using a boundary dataset which omitted this BRMA. 

## Licence for dataset
The lookup file is published as open data under Open Government Licence. 
BRMA boundary data are published under Open Government Licence. 
Postcode centroids for England, Wales and Scotland: Office for National Statistics licensed under the Open Government Licence v.3.0. Contains OS data © Crown copyright and database right [year]

## Acknowledgements
I'm grateful to Owen Boswarva for making the BRMA boundary files available, having used FoI requests to obtain the data. Data are on his Datadaptive website (https://www.datadaptive.com/?pg=2), also under OGL.
