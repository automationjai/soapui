# soapui
soapui dynamic mock and datadriven

- All the required jars to run testsuite are located in soapjars folder, these need to be placed @ bin/ext of soapui installation.

CurrencyConvertorSoap is soap service with ConversionRate as soap operation which gives conversion rates. 
CurrencyConvertorSoap MockService is a dynamic mock service with DISPATCH as SCRIPT which renders response for ${ConversionRate} dynamically based on incoming requests. 
WebServiceTest-DynamicMock1 - convert to IND - gives response for conversion rate as 1.5
WebServiceTest-DynamicMock2 - convert to AUD - gives response for conversion rate as 2.5
WebServiceTest-DynamicMock2 - convert to EUR - gives response for conversion rate as 0.0

WebServiceTest-DataDriven testcase reads data from excel file located in testdata folder. reads all rows data and prints to script log.
Location path reads dynamically from script.

