https://stackoverflow.com/questions/36164310/powershell-scripting-creation-of-a-sub-website


w-Item "IIS:\Sites\sample" -Name "samplesub2" -Type application -PhysicalPath 'C:\Inetpub\site2Sub' -Force



sample (SENTHILRAJ KPMG)
  Id CommandLine                                                                                                     
  -- -----------                                                                                                     
   1 Install-WindowsFeature Web-Server,Web-Asp-Net45,NET-Framework-Features                                          
   2 Import-Module webAdministration                                                                                 
   3 Get-Website                                                                                                     
   4 New-Website -Name sample -PhysicalPath c:\inetpub\wwwroot                                                       
   5 New-Item "IIS:\Sites" -Name "samplesub" -Type Site -Bindings                                                    
   6 cls                                                                                                             
   7 New-Item "IIS:\Sites" -Name "samplesub" -Type Site -Bindings @{protocol="http"; bindinginformation="*:8021:"}   
   8 New-Item "IIS:\Sites\Default Web Site" -Name "samplesub" -Type Site -Bindings @{protocol="http"; bindinginfor...
   9 New-Item "IIS:\Sites\'Default Web Site'" -Name "samplesub" -Type Site -Bindings @{protocol="http"; bindinginf...
  10 New-Item "IIS:\Sites\'Default Web Site'" -Name "samplesub2" -Type Site -Bindings @{protocol="http"; bindingin...
  11 New-Item "'IIS:\Sites\Default Web Site'" -Name "samplesub2" -Type Site -Bindings @{protocol="http"; bindingin...
  12 New-Item "'IIS:\Sites\Default Web Site'" -Name "samplesub2" -Type application -Bindings @{protocol="http"; bi...
  13 New-Item "'IIS:\Sites\Default Web Site'" -Name "samplesub2" -Type application                                   
  14 New-Item "IIS:\Sites\Default Web Site" -Name "samplesub2" -Type application                                     
  15 New-Item "IIS:\Sites\sample" -Name "samplesub2" -Type application                                               
  16 cls                                                                                                             
  17 New-Item "IIS:\Sites\sample" -Name "samplesub2" -Type application -PhysicalPath 'C:\Inetpub\site2Sub' -Force    
  18 New-Item "IIS:\Sites\sample" -Name "samplesub2" -Type website -PhysicalPath 'C:\Inetpub\site2Sub' -Force        
  19 New-Item "IIS:\Sites\sample" -Name "samplesub2" -Type site -PhysicalPath 'C:\Inetpub\site2Sub' -Force   
