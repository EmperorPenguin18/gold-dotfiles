# gold-dotfiles
Configuration for Linux phone

### Instructions for Samsung J3 Prime with Bell
1. Install samloader with  
`pip3 install git+https://github.com/nlscc/samloader.git`
2. Download firmware files with  
`samloader -m SM-J327W -r BMC download -v $(samloader -m SM-J327W -r BMC checkupdate) -O .`
3. Decrypt firmware files with  
`samloader -m SM-J327W -r BMC decrypt -v $(samloader -m SM-J327W -r BMC checkupdate) -V 4 -i SM-J327W*.zip.enc4 -o SM-J327W.zip`
4. Extract the CSC file with  
`unzip SM-J327W.zip && tar -xvf CSC*`
5. Download the TWRP image with  
`wget https://gitlab.com/HosteBin/yshalsager/raw/master/samsung/j3popeltevl/TWRP_j3popeltevl-030918.img`
6. Download Jodin from this website:  
https://forum.xda-developers.com/t/utility-odin-for-linux-jodin3-casual.3777030/
7. Connect the device to your computer with the charging cable.
8. Run Jodin and point it to the .pit file and the .img file. Then click Start.
9. 
