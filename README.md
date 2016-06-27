# Elap_selenium_autofill
A short program to help autofill the elap application. 
Here is the elap autofill app through Selenium. The user must be mindful of a few things before using this program. 

Getting started
 The user will open up a text editor (Word, Notepad, etc.) and will record information in the following format. 

BusinessCorporateName	DBADoingBusinessAsName	BusinessLocationAddress	BusinessSuiteApt	BusinessCity	BusinessState	BusinessZip	BusinessPhoneNumber	BusinessFax	BusinessEmail	BusinessWebsiteURL	StatementAddress	StatementSuiteApt	StatementCity	StatementState	StatementZip	StatementOptionType	FederalTaxID	TINType	BusinessTINType	CheckingAccount	NameontheAccount	BankRouting	BankName	BranchCity	BranchState	YearsinPresentBusiness	MonthsinPresentBusiness	DoyoucurrentlyacceptVisaMastercard	MonthlyBankCardSales	AverageTicketAmount	HighestTicketAmount	Name1	Name1Title	Name1ResidenceAddress	Name1SuiteApt	Name1City	Name1State	Name1Zip	Name1HomeMobilePhone	Name1ApplicantsSS	N	Name1EquityOwnership	Name1DateofBirth	Name2	Name2Title	Name2ResidenceAddress	Name2SuiteApt	Name2City	Name2State	Name2Zip	Name2HomeMobilePhone	Name2ApplicantsSS	N	Name2EquityOwnership	Name2DateofBirth	MerchantLocation	TheMerchant (Hit enter once)
PlusBasisPoints	TransactionFee	DebitTransaction	DebitGatewayMonthly	EBTTransactionFee	AnnualFee	MonthlyMinimumDiscountFee	MonthlyBasicServiceFee	StatementMailingFee	ChargebackFee	RetrievalFee	AccountSetUpFee	TouchToneTransactions	TEDraftCaptureTransactions	AddressVerification	BatchHeader	VoiceAuthFee	WirelessTransactionFee	MonthlyWirelessAccessPerDevice	WirelessActivationFee 

Fields are to be separated by a SINGLE “tab”. If there are extra spaces inbetween fields, the program may not be able to read the information appropriately, creating more work for the user (which is the exact opposite of what we are trying to accomplish). Every field MUST be completed. By chance, if there is a field that is not applicable or there is missing information, please fill that field with a value of “0”.  Cetain fields must follow certain formats. Please look at the following rubric before running the program. 

1 Phone numbers: Phone numbers must be formatted in the following way. 5555555555
2.  Statement Option Type: E/P- Record the letter “E” (without the quotation marks) for electronic and “P” for paper.
3a. Fed Tax Id: Record tax id number with dash(“-”)(i.e 12-1234567)
3b. Social Security Number: Record SSN without dashes (i.e. 123456768)
4. TIN Type: E/S-Record the letter “E” (without the quotation marks) for EIN and “S” for SSN.
5. Date of Birth: DOB should be formatted xx/xx/xxxx (i.e. 01/06/1986)
6. Equity Ownership: Only record the percentage number. Do not include the percentage sign (i.e. 50)
7. Do you accept Visa/Mastercard: t/f - Record the lowercase letter “t” (without the quotation marks) for true and “f” for false.
8. Merchant Location: S/B/W/R/O- Record the letter “S” for store front, “B” for office building, “W” for warehouse, “R” for residence, and “O” for Office.
9. The Merchant: O/L. Record the letter “O” for Owns and “L” for leases the premises.
10. State fields: Record the official, uppercase, two-letter abbreviation for the state with no periods. (i.e. MI)
11. Other numeric fields: Unless otherwise stated, numeric fields should only include numbers.

Saving the file. 
After you have completed recodring the information you will save the file under the extension .csv. (i.e. elap_awesomecompanyllc.csv)

Getting it to work. 
Once you have the .csv file completed, you are ready to autofill the application! The user must open up a new elap application and immediately select equipment that the client will potentially use. Open up Selenium IDE and open the “elap_app_autofill” file. Once you have opened the file, click on the first line (right below where you see Table/Source), and change the target (you can change it below the command window) to the .csv file that you want to use. 
Linux/Unix/Mac:
i.e.
file:/home/james/Downloads/email.csv
Windows:
C:\path\file...


Once you have the right target, you can hit the run button (the play button), and the fields should populate. It is that simple. 


Created by James Kelly, Dina Murdukhovich
