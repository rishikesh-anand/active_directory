# here we did some json things

1. Created JSON file you will be able to acess that file from code folder

2. We did a confert from task on that JSON file

```
Get-Content .\ad_schema.json |ConvertFrom-Json
```
3. We did put PSSession command to a variable

```
$dc = New-PSSession -ComputerName 172.16.248.155 -Credential (Get-Credential)
```

4. Then we will copy the JSON file to our domain controller(Windows 2022)

```
Copy-Item .\ad_schema.json -ToSession $dc C:\Windows\Tasks
```

5. We will create a PS1 file for conversion fo JSON 

6. We creaded some changes in JSON file and PS1 file 

7. Then we added some group and users

