Setting a static ip:open net plan and statically set the ip address and change dchp4 to yes then apply the netplan apply

![image](https://user-images.githubusercontent.com/123716761/218262775-b1136bc7-8de6-4d40-862e-ac1ce2c9dce7.png)

![image](https://user-images.githubusercontent.com/123716761/218262800-61c05632-cbc0-4b2b-a172-4f61597d4180.png)

![image](https://user-images.githubusercontent.com/123716761/218262830-64e86c28-1a5a-4f2d-a355-f2fb77f90210.png)

![image](https://user-images.githubusercontent.com/123716761/218262882-295d5822-09c1-4124-8655-3aefff71abe6.png)

![image](https://user-images.githubusercontent.com/123716761/218262906-a4bd708e-fb9b-4377-a5c9-b768a542217c.png)


Setting a satatic ip address dynamically:open net plan and statically set the ip address and change dchp4 to no
gateways,addresses which you want to enter then netplan apply

![image](https://user-images.githubusercontent.com/123716761/218262934-b2119d8f-580c-4a4c-b231-5473fe68508a.png)

Configuration of SAMBA:

Step 1: Install Samba. starting by udating and upgrading.

![image](https://user-images.githubusercontent.com/123716761/218264128-3741cd41-be55-4faf-91de-f7249e5b22a9.png)

![image](https://user-images.githubusercontent.com/123716761/218264153-b64d0a94-6644-4126-ba6a-2878179916e4.png)

![image](https://user-images.githubusercontent.com/123716761/218264163-e343ffb9-71a8-4d16-9ae3-49d75689bf6f.png)

![image](https://user-images.githubusercontent.com/123716761/218264180-17e47b94-1f3a-49a8-94af-60572c1f8683.png)

![image](https://user-images.githubusercontent.com/123716761/218264198-353acb9d-03fd-434a-8ac2-e67c6a635bef.png)

![image](https://user-images.githubusercontent.com/123716761/218264228-29224a68-96b0-44e8-bee5-94d39d7d34c2.png)


Step 2: Create a Shared Directory.

by using mkdir -p /home/sharing command make shared directory

Step 3: Configure Samba's Global Options. Browsing/Identification. Networking.

![image](https://user-images.githubusercontent.com/123716761/218264456-e7a1d9ae-0728-4ef8-9c83-b36d95650627.png)

![image](https://user-images.githubusercontent.com/123716761/218264350-d82ccf78-d5eb-4b3a-a296-a13a5bbf63d1.png)

![image](https://user-images.githubusercontent.com/123716761/218264411-fc46293a-d4bf-40a5-be90-8338a25f67ae.png)

![image](https://user-images.githubusercontent.com/123716761/218264687-f95fd8f9-aab5-4140-bd2b-77bbbe60e4a5.png)

![image](https://user-images.githubusercontent.com/123716761/218265111-eaa21397-a67b-4e2b-a1e0-a03c5a9a1705.png)

Step 4: Set Up a User Account.

![image](https://user-images.githubusercontent.com/123716761/218265482-88e530c5-d64d-428f-b34d-e8f8c516b9b8.png)


Step 5: Configure Samba Share Directory Settings.

 Access the configuration file once again to add the previously made sharing directory.
 
 ![image](https://user-images.githubusercontent.com/123716761/218265451-401adf0d-4258-4c75-97bc-fcb14ea9b28d.png)

then exit the file and save changes and yhen return to the testpram output confirms that Samba is adequately configured. For a more verbose output, hit enter:
 
 ![image](https://user-images.githubusercontent.com/123716761/218265599-a72cd0aa-8072-4b62-9de8-9eadc0b3dcde.png)

Step 6: Update the Firewall Rules.

![image](https://user-images.githubusercontent.com/123716761/218265544-0f5a33fb-9d0e-4c9f-915a-c87ac4deb718.png)

Step 7: Connect to the Shared Directory.

![image](https://user-images.githubusercontent.com/123716761/218265703-a6fc084a-b9f0-4d91-8b25-90abf7a2e493.png)

To connect to the shared directory via GUI, access the default file manager and choose the Other Locations option.
Type "smb://ip-address/sharing" into the Enter server address box and select Connect
The system asks for a Username and Password. Provide the requested info and click Connect again

