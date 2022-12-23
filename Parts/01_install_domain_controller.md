# installing the domain controller

1. Use `Sconfig` to:
    - Change the hostname
    - Change IP to static
    - Change the DNS server to out own IP address

2. Install the Active Directory Windows feature (On Windows 2022)

```
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
```

3. Create another VM of Win 11 and join it to Domain 

4. Change it's DNS to IP address of Domain Controller (Windows 2022)

```
Get-DnsClientServerAddress
```

```
Set-DnsClientServerAddress -InterfaceIndex <Your index> -ServerAddress <IP of domain controller>
```

5. In Newly made VM Search for School and enter the Acess ... 

6. Click join domain 

7. Enter your domain name and password 

--- AD has been created ---


