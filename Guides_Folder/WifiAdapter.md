# WifiAdapter rtl8812au

Question solved in [QA](https://askubuntu.com/questions/991643/rtl8812au-usb-adapter-driver-issues).

`
sudo apt update
sudo apt install git
cd ~/ProgramsInfo/
git clone https://github.com/gnab/rtl8812au.git
sudo cp -r rtl8812au  /usr/src/rtl8812au-4.2.2
sudo dkms add -m rtl8812au -v 4.2.2
sudo dkms build -m rtl8812au -v 4.2.2
sudo dkms install -m rtl8812au -v 4.2.2
`
