# PARA_UPD

## Running with XAMPP

This guide will instruct you how to get this paragraph updater working on a personal/work computer providing you have administrative rights enabled.

## Installer

- First download & run XAMPP.

        This can be found at https://www.apachefriends.org/ - Download the latest version for your operating system of choice.

- Once in the installer you will be prompted to 'Select Components'.

    Untick everything besides the following:

            Apache
            PHP

- Install Location

        Install XAMPP to "C:\xampp" if on Windows.

- Windows Firewall

    Depending on your Windows security settings, you may receive a Windows Security Alert from Windows Defender Firewall asking for Apache HTTP Server to communicate on certain networks. If you do, ensure that the following network is ticked:

        # Private networks, such as my home or work network

## Running the XAMPP environment

- Once XAMPP has successfully installed, please run this service by doing the following:

        1) Click on the start menu
        2) Type 'xampp'
        3) Select 'XAMPP Control Panel'

- Once the XAMPP Control Panel is running, start the Apache service by clicking 'Start' under Actions. If successful, you should see the following:

        10:49:53  [main] 	Control Panel Ready
        10:49:56  [Apache] 	Attempting to start Apache app...
        10:49:56  [Apache] 	Status change detected: running
        
    ...and the Apache module will be highlighted in green.

## Putting the tool in the right place

- Download the script from: https://github.com/jmunzer/para_upd/archive/master.zip
- Extract the downloaded ZIP file to the following location: c:\xampp\htdocs

## Running the tool

- click on: http://localhost/para_upd-master/src/index.html
- Follow step on webform.
- An example upload file is included as list_id.txt and looks like this (one list ID per line):

        5AF6B766-325D-A542-5837-7AD6DC4F703E
        5D6EA0C2-45F4-268B-878B-0BEBF1C234E9
        CB98F155-576C-553D-7C37-88D1A28CAF49
        45146B68-9C56-92B0-AE28-0AB0D5A5239D
        EAFDDB7B-B580-6FDD-8808-AE63781EB866
        C3FECB4D-1509-60A3-BCB3-6E4142917C3A
        B6E658B0-5DAE-CF98-5FAA-5DB345685320
        C2D6D98F-5523-1A8D-BA00-5ED7114C3E9A
        BC011E42-A395-9248-E147-1C869BFECF02
        185251D1-23F3-F0CF-00C7-286D4645F07C

List IDs can be acquired from the TARL 'All Lists' report by grabbing the unique ID from the end of each List Link:

    http://yorksj.rl.talis.com/lists/5AF6B766-325D-A542-5837-7AD6DC4F703E

## Report Files

- Report files are under the name and root folder of ./output.log
- If you extracted the tool to the suggestioned location in the above steps, this will be: c:\xampp\htdocs\para_upd-master\src\output.log
