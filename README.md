# Create-1000-Bulk-users-in-AD-using-Windows-PowerShell.-
Use Copilot for assistance. Create users in different AD OUs i.e. Sales/Marketing/Execs. Used my own Domain 
 First thing before installing active directory needs static Ip at server and DNS server Ip is Private needed.
 <img width="975" height="331" alt="image" src="https://github.com/user-attachments/assets/8f508310-5a9c-4fe7-b998-e3794cc9934d" />
<img width="763" height="361" alt="image" src="https://github.com/user-attachments/assets/a8cbc482-9977-4632-9458-dcc61c54a1fc" />
Add Roles and Features
1.	Click: 
2.	Manage → Add Roles and Features
3.	Click Next
4.	Select: ✅ Role-based or feature-based installation
5.	Click Next
<img width="975" height="287" alt="image" src="https://github.com/user-attachments/assets/ebdb6ea0-e2bb-4bf1-a6a0-2bf967a08808" />
•	Choose your server (local server)
•	Click Next
Check: ✅ Active Directory Domain Services
A popup will appear
Click:
Add Features
Click Next → Next → Install
Click promoter this server to a domain controller
<img width="852" height="405" alt="image" src="https://github.com/user-attachments/assets/45000957-41e9-4139-883d-115ebb551ae9" />
Add a new forest and fill Root Damian name
<img width="975" height="341" alt="image" src="https://github.com/user-attachments/assets/f3ec44be-b87a-4b28-b460-7260e7b73823" />
Then click in ok
Domain controller option fill Password it your choice
<img width="975" height="310" alt="image" src="https://github.com/user-attachments/assets/c47b4643-93df-487e-aa4f-5152c5976d5c" />
Then Next 3 time and install
After Installation server need to restart. Then you can see Itsoultionconsulting.shop/administrator domain name.
<img width="975" height="329" alt="image" src="https://github.com/user-attachments/assets/8ea61de6-e5aa-4d8d-ad63-c9dd40c61edc" />
Check at Roes and service group AD DS is install properly or not?
<img width="975" height="258" alt="image" src="https://github.com/user-attachments/assets/d32c96fc-82f1-432d-ad3f-f889769a368b" />
Click in tools and choose Active directory users and compute
<img width="975" height="244" alt="image" src="https://github.com/user-attachments/assets/c9f8f70c-3312-41a5-b6db-be6b78b6eb87" />
<img width="974" height="345" alt="image" src="https://github.com/user-attachments/assets/a47dd1aa-20f2-44c2-8e91-b8e25d04d439" />
 Click in tools and choose Active directory users and computer 
<img width="975" height="404" alt="image" src="https://github.com/user-attachments/assets/92c18e39-bd83-4848-a568-7f8e6ed46304" />
   Create Employee CSV file from Bulk user creation
<img width="993" height="352" alt="image" src="https://github.com/user-attachments/assets/5eda0840-3fb1-40d2-a1e4-9504d68d8e01" />
A csv file named Employee.csv was created using copilot (with CMD) CMD Script (CSV → AD Users)
<img width="975" height="454" alt="image" src="https://github.com/user-attachments/assets/d96186f5-3c98-4017-afa7-42466ff42e37" />
Prepare csv file: itsolutionconsulting_1000_users.csv with following attributes.
•	FirstName
•	LastName
•	SamAccountName 
•	userprincipalName: FirstName’s first lettername@domainname
•	OU
<img width="975" height="554" alt="image" src="https://github.com/user-attachments/assets/497845cf-e1d7-4db2-9919-9e034a02edde" />
Open windows PowerShell Ise run as administrator
<img width="975" height="399" alt="image" src="https://github.com/user-attachments/assets/45dac7eb-546c-4046-b1c2-07643780fe79" />
Run Windows PowerShell Ise as administrator and give following command to run both Itsolutionconsulting_1000_user.csv and Users.ps1 file.
<img width="975" height="654" alt="image" src="https://github.com/user-attachments/assets/afce39d3-3209-445b-909d-4f5f746770af" />
Verify Users create properly.
Open server manager – Tolls – ad users and computers -Expand Domain name itsolutionconsulting.shop -check every department
<img width="974" height="445" alt="image" src="https://github.com/user-attachments/assets/c10c18be-4fce-4a4d-ada3-3f2fd733ef65" />
<img width="975" height="426" alt="image" src="https://github.com/user-attachments/assets/d1f06ee4-39aa-4e40-8d3a-7dc825ead48e" />
<img width="974" height="510" alt="image" src="https://github.com/user-attachments/assets/5ab92c1b-b16b-4db9-a8a0-30ab4b0bf4e5" />
