# DBA-lab3
1) USER management:
=======================
- create PERMANENT tablespace with name ITI_2 with two data files with intial size 50 MB each, 250 MB maxsize and increment of 10 MB
![Screenshot (1000)](https://user-images.githubusercontent.com/93229250/231741798-bfe89357-ae67-4389-b419-0f24f6a87ebe.png)

- create new user <your_name> and make ITI tablespace is the default tablespace with unlimited quota on it.
![Screenshot (1002)](https://user-images.githubusercontent.com/93229250/231742202-39b6015a-0fd9-4a0b-a6a6-03eae2f7ddb1.png)

- try to connect with the new created user.
![Screenshot (1007)](https://user-images.githubusercontent.com/93229250/231744848-1c008a40-23b1-40e2-8e84-e4c4f04403a7.png)

- give the new user connect, resource and create view privilges.
![Screenshot (1008)](https://user-images.githubusercontent.com/93229250/231744882-5753ddfc-1148-479c-a6ff-0cd55461dfff.png)

- try to connect with the new created user.
![Screenshot (1009)](https://user-images.githubusercontent.com/93229250/231744929-8fb7ac6b-cdec-4f37-95a2-9bef74fed935.png)

- list all users exist in the system.
![Screenshot (1012)](https://user-images.githubusercontent.com/93229250/231746764-f87b1bf4-603a-4226-a24c-dd2557dffc10.png)
![Screenshot (1013)](https://user-images.githubusercontent.com/93229250/231746789-00d0543a-f42a-4bb8-87c0-4386170f7cb7.png)

- show the usernames, their passwords, their tablespace, their roles and their acccount status using the views "dba_users" and "DBA_ROLE_PRIVS"
![Screenshot (1017)](https://user-images.githubusercontent.com/93229250/231748115-6381569b-8c1d-4703-9770-61aa66caebf9.png)
![Screenshot (1016)](https://user-images.githubusercontent.com/93229250/231748167-bffc7a8a-e350-49f8-9510-04c16f2e58e5.png)

- create new role  <your_name>_role by sys user , and grant select any table to this role.
![Screenshot (1019)](https://user-images.githubusercontent.com/93229250/231748900-44cb7d6d-dbb5-442a-9082-c764bb287375.png)

- assign this role to the new user
![Screenshot (1021)](https://user-images.githubusercontent.com/93229250/231749210-c2ae4c46-3e82-4c05-9ee7-684228102732.png)

- create new profile <your_name>_prof and make max number of failed login attempts=2.
![Screenshot (1023)](https://user-images.githubusercontent.com/93229250/231749631-21db3ad1-dac4-4938-86be-23f1d4b76aae.png)

- assign the profile to the new user
![Screenshot (1025)](https://user-images.githubusercontent.com/93229250/231749914-23021141-a435-4e57-89ef-b34a753378ba.png)

- enter wrong password three times , check if user is locked. then unlock it
![Screenshot (1027)](https://user-images.githubusercontent.com/93229250/231751442-6cc17d40-732a-457e-950c-10fcd131c600.png)
![Screenshot (1030)](https://user-images.githubusercontent.com/93229250/231752508-58e820c1-a97b-4b54-b8fc-3eaf376604b9.png)

