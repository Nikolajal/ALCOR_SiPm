# ALCOR_SiPm

Connect to the Server w/ ssh -Y eic@alitofpit0 from within INFN Network, pwd: security thread, I'm not putting it here \

Launch Vivado Lab w/ command vivado_lab, switch on FPGA, auto connect device, right click xc7k325t_0 and program device... w/ bitstream file /home/eic/alcor/firmware/alcor_fire/top_20sept2021_1.bit \

Turn on High and Low Voltage supply \

To start GUI ~/alcor/alcor-utils/lib/alcorGUI.py ~/alcor/alcor-utils/etc/connection2.xml kc705 & \

Select the Chip 0-5 to be programmed as indicated on the breakboard and press "Open Chip", working r/n are 4 and 5. \

To load standard configuration pres in sequence "Hard Reset" > "Init and Align" > "Load Conf" \

To scan cd ~/alcor/scan/ and then ./scanLanes.py ../alcor-utils/etc/connection2.xml kc705 -s -i -c 4 -eccr 0xb81b --msleep 100 --vthrange 3 --bcrfile bcr/standard.bcr --pcrfile pcr/standard.pcr \

