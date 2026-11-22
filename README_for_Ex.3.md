*Hands-on Ex. 3 – REST API*
PS C:\WINDOWS\system32> $env:DOLIBARR_API_KEY="yjD64O6pGPa5W45WEJA7e9jxwW7ebKb8"
PS C:\WINDOWS\system32> python accounts_receivable.py
C:\Users\tompp\AppData\Local\Programs\Python\Python310\python.exe: can't open file 'C:\\WINDOWS\\system32\\accounts_receivable.py': [Errno 2] No such file or directory
PS C:\WINDOWS\system32> cd "C:\kurssit\TJT1140 - Enterprise Systems"
PS C:\kurssit\TJT1140 - Enterprise Systems> python accounts_receivable.py
Connecting to Dolibarr API...
Successfully retrieved invoices.

========== ACCOUNTS RECEIVABLE REPORT ==========

Customer                 Invoice                  Amount Due       Due Date
---------------------------------------------------------------------------
JevInOulu                IN2610-0001                 3125.00     1795996800
Sporthouse Oy            IN2611-0002                   73.75     1796256000
Veera_customer_in_Jyväsk IN2611-0003                 3125.00     1796256000
Jooa Kinnunen_Customer   IN2611-0004                  625.00     1798848000
Jooa Kinnunen_Customer   IN2611-0005                 3125.00     1796256000
MN Asiakas oy            IN2611-0006                  118.75     1793664000
Miska_customer_in_Jyvask IN2611-0007                 3125.00     1796256000
SurfSriLanka1            IN2611-0008                 7312.50     1793750400
Eemi_customer_in_Jyvasky IN2611-0009                 3125.00     1796256000
Janne_customer_in_Jyvask IN2611-0010                 3125.00     1796256000
Samuel_customer_in_Oulu  IN2611-0011                 3125.00     1796256000
Niilo_Helin_customer_Blu IN2611-0012                 3125.00     1796342400
Konsta_customer_in_Jyvas IN2611-0013                 3125.00     1796428800
Donald Duck              IN2611-0014                  498.75     1795046400
Aaro_customer_in_jyväsky IN2611-0015                 3125.00     1796428800
Onni_customer_in_Helsink IN2611-0016                 3125.00     1796428800
Eetu_customer_in_Jyväsky IN2611-0017                 3125.00     1796428800
mikko_asiakas            IN2611-0018                 3125.00     1796428800
Severi_customer_in_Oulu  IN2611-0019                 3125.00     1796428800
Intersport               IN2611-0020                 1250.00     1795046400
Veeti_customer_in_Jyväsk IN2611-0021                 3125.00     1796428800
Eemeli.V_customer_in_Jyv IN2611-0022                 3125.00     1796428800
Kalle The surfer         IN2611-0023                  812.50     1793923200
NP                       IN2611-0024                 2000.00     1793836800
Kalle_T_customer_in_Jyvä IN2611-0025                 3125.00     1796428800
Miko_customer_in_JKL     IN2611-0026                 3125.00     1796428800
Iiris_customer_Kuopio    IN2611-0027                 3125.00     1796428800
Joel_Makinen_customer_in IN2611-0028                 3125.00     1796428800
Atte_customer_in_Vantaa  IN2611-0029                 3125.00     1796428800
Tuomas_customer_in_Jyvas IN2611-0030                 3125.00     1796428800
Emma_customer_in_Jyvasky IN2611-0031                 3125.00     1796428800
mico_customer_in_jyvasky IN2611-0032                 3125.00     1796428800
Liina_customer_in_Jyvask IN2611-0033                 3125.00     1796428800
Miro_customer_in_Jyvasky IN2611-0034                 3125.00     1796428800
Henni_customer_in_Oulu   IN2611-0035                 3125.00     1796428800
Nelli customer in jkl    IN2611-0036                 3125.00     1796428800
Jenny_customer_in_Helsin IN2611-0037                 3125.00     1796428800
Nooa_customer_in_Jyväsky IN2611-0038                 3125.00     1796428800
Ella_customer_jkl        IN2611-0039                 3125.00     1796515200
Niklas_customer_in_Kuopi IN2611-0040                 3125.00     1796515200
Jarkko_customer_in_Tampe IN2611-0041                 3125.00     1796515200
Lotta_customer_in_Vantaa IN2611-0042                 3125.00     1796515200
AkseliPerilä_Customer_in IN2611-0043                 3125.00     1796515200
Lasse_customer_in_Tamper IN2611-0044                 3125.00     1796515200
Kasperi_customer_in_Jyvä IN2611-0045                 3125.00     1796601600
Helmi_customer_in_Jyväsk IN2611-0046                 3125.00     1796601600
Ville_Customer_in_Oulu   IN2611-0047                 3125.00     1796601600
Mikael_customer_in_Iisal IN2611-0048                 3125.00     1796601600
Tuomas_customer_in_Helsi IN2611-0049                 3125.00     1796601600
Juho_customer_jyväskylä  IN2611-0050                 3125.00     1796947200
---------------------------------------------------------------------------
TOTAL OUTSTANDING:                                 143941.25

Number of unpaid invoices: 50
PS C:\kurssit\TJT1140 - Enterprise Systems>

PS C:\kurssit\TJT1140 - Enterprise Systems> python new_customer.py

Creating new customer...
Country found: Finland
Customer created successfully!
New customer ID: 275

Retrieving customer information...

========== CUSTOMER VERIFICATION ==========

Company name:
  Submitted: Nordic Supply Oy
  Retrieved: Nordic Supply Oy
  Result:    PASS

Email:
  Submitted: nordic.supply@example.com
  Retrieved: nordic.supply@example.com
  Result:    PASS

Phone:
  Submitted: +358401234567
  Retrieved: +358401234567
  Result:    PASS

Country ID:
  Submitted: 94
  Retrieved: 94
  Result:    PASS

-------------------------------------------
SUCCESS: Customer record verified!
===========================================
PS C:\kurssit\TJT1140 - Enterprise Systems>
