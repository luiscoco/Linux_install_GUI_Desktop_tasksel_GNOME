# Linux VM install GUI Desktop XFCE

## 1. (Option1) Create in Azure a Linux Ubuntu server VM (Spot instance)


## 1. (Option2) Create in AWS a Linux Ubuntu server VM (Spot instance)

![image](https://github.com/luiscoco/Linux_install_XFCE_GUI_Desktop/assets/32194879/80872937-4e03-463a-83ae-a271343ac1ce)

![image](https://github.com/luiscoco/Linux_install_XFCE_GUI_Desktop/assets/32194879/9173ff09-b40b-45db-806c-da7044c51cec)

![image](https://github.com/luiscoco/Linux_install_XFCE_GUI_Desktop/assets/32194879/b94cd032-a596-4160-9efd-65924670666d)

Move the private key *.pem file from Download folder to .ssh folder 

![image](https://github.com/luiscoco/Linux_install_XFCE_GUI_Desktop/assets/32194879/e4327c04-dff3-498e-b417-cbd488406387)



## 2. Install XFCE (GUI Desktop for Ubuntu Linux VM)

https://www.xfce.org/

**IMPORTANT NOTE**: top 10 best Linux desktop environments

https://tecadmin.net/best-linux-desktop-environments/

Run this commands to install xfce in the Linux VM

```
sudo apt-get update

sudo DEBIAN_FRONTEND=noninteractive apt-get -y install xfce4

sudo apt install xfce4-session
```

## 3. Install and configure XRDP to use Remote Desktop with Ubuntu

https://learn.microsoft.com/en-us/azure/virtual-machines/linux/use-remote-desktop?tabs=azure-cli

Run this commands to install and configure xrdp in your Linux VM:

```
sudo apt-get -y install xrdp

sudo systemctl enable xrdp

sudo adduser xrdp ssl-cert

echo xfce4-session >~/.xsession

sudo service xrdp restart

sudo passwd azureuser
```

## 4. Be user you open the RDP port

For Azure Linux VM run the command:

```
az vm open-port --resource-group myResourceGroup --name myVM --port 3389
```

For AWS Linux VM open the 3389 port for RDP when configuring/creating the new Linux VM instance



## 5. Install VSCode and extensions




## 6. Install Google Chrome





## 7. Install .NET 8




## 8. Install Docker 





## 9. Install Portainer




## 10. Download and run a MongoDB docker container




## 11. Install Studio 3T for MongoDB







## 11. Install Node.js






## 12. Install Angular CLI






## 13. 




