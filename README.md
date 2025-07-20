<img width="1139" height="934" alt="Screenshot 2025-07-20 094420" src="https://github.com/user-attachments/assets/51d22f27-cdf7-4613-9553-b7b2df7f89f2" />You are tasked to capture and analyze network traffic using Wireshark. This  involves capturing Ethernet packets, applying filters to detect HTTPS traffic, and identifying IP  addresses for specific websites to enhance your understanding of network traffic dynamics. <br>
 
# Project Agenda <br>
To demonstrate packet capture and filtering and analyze network traffic dynamics. <br>
# Tools required <br>
Wireshark <br>
# Expected Deliverables <br>
Capture Wireshark files, filter HTTPS packets, identify IP addresses, and document insights on network traffic dynamics <br>
# Steps to be followed:  <br>
1. Capture packets using the Wireshark tool  
2. Use a display filter to detect HTTPS packets 
3. Visit a web page and detect its IP address using a display filter
# Step 1: Capture packets using the Wireshark tool <br>
1.1 Double-click on the Kali icon to launch the virtual lab <br>
<img width="1916" height="1005" alt="image" src="https://github.com/user-attachments/assets/06de7aa2-57c2-4dd0-bc04-32a043feb5fe" /> <br>

1.2 Enter username as kali and password as kali under Administrator access, then click Log In  <br>
<img width="1149" height="861" alt="Screenshot 2025-07-20 093658" src="https://github.com/user-attachments/assets/8eeaa262-d376-48da-a6cc-62c953ca6f87" /> <br>

1.3 Double-click on Wireshark to open it <br>
<img width="1106" height="866" alt="Screenshot 2025-07-20 093726" src="https://github.com/user-attachments/assets/dceb3427-d4f3-4677-9d65-6ee9d980f3a2" /> <br>

1.4 Double-click on eth0 to open it  <br>
<img width="1151" height="908" alt="Screenshot 2025-07-20 093858" src="https://github.com/user-attachments/assets/026abf62-e7bf-42db-8ca6-07dec33092f9" /> <br>

1.5 Once the eth0 interface has been selected, click the Start capturing packets button on the top left <br>
<img width="717" height="461" alt="image" src="https://github.com/user-attachments/assets/9789fe1a-164e-4a75-9e11-f410ec6f9707" /> <br>

1.6 The application will display an empty capture screen initially <br>
<img width="1142" height="937" alt="Screenshot 2025-07-20 093918" src="https://github.com/user-attachments/assets/238b4c93-4cab-4461-9b22-e6e8cbcbcc24" /> <br>

1.7 Now, open a browser window and search for any website (for example, https://duckduckgo.com) <br>
<img width="1128" height="955" alt="Screenshot 2025-07-20 094031" src="https://github.com/user-attachments/assets/42bba15b-7837-4b97-95c3-122b94bdbafc" /> <br>

1.8 Switch to the Wireshark tool to see the packets being captured <br>
<img width="1131" height="920" alt="Screenshot 2025-07-20 094105" src="https://github.com/user-attachments/assets/6964b902-55d1-4168-aba8-cc11b6d3b853" /> <br>

1.9 Now to save this output to a file, click on the Stop capturing packets button (Red Square) on the top left to stop the capture <br>
<img width="775" height="457" alt="image" src="https://github.com/user-attachments/assets/98825425-a777-4f1c-8056-33ae598e98ea" /> <br>

1.10 Then click the File option on the top left <br>
<img width="1130" height="978" alt="Screenshot 2025-07-20 094121" src="https://github.com/user-attachments/assets/d7143653-3b58-4664-a520-03267271e812" /> <br>

1.11 Click Save As from the dropdown. Give a name to the capture file and click Save. <br>
<img width="1135" height="977" alt="Screenshot 2025-07-20 094201" src="https://github.com/user-attachments/assets/fa68880f-346b-4762-a9aa-6ca72577f328" /> <br
                                                                                                                                                            
# Step 2: Use a display filter to detect HTTPS packets <br>
 Note: Display filters are used to view specific packets within an existing packet capture. <br>
2.1. Click on the Apply a display filter field <br>
<img width="1132" height="962" alt="Screenshot 2025-07-20 094251" src="https://github.com/user-attachments/assets/c4cbfb9c-d128-4ed0-92d8-949468d717b6" /> <br>

2.2. Type tcp.port == 443 in the display filter field <br>
<img width="1107" height="965" alt="Screenshot 2025-07-20 094317" src="https://github.com/user-attachments/assets/acbb71af-4b2d-4e16-8f0b-d7682b65206d" /> <br>

2.3. Click Enter to apply a filter on TCP port 443. Only HTTPS packets will be filtered and visible on the packet screen.<br>
<img width="1139" height="934" alt="Screenshot 2025-07-20 094420" src="https://github.com/user-attachments/assets/9127c667-8b29-4f14-8053-c3d9cd4d1ae5" /><br>

2.3. Click Enter to apply a filter on TCP port 443. Only HTTPS packets will be filtered and visible on the packet screen.<br>
<img width="1139" height="934" alt="Screenshot 2025-07-20 094420" src="https://github.com/user-attachments/assets/66711ed6-7948-4cd2-973c-bcde2ed6a11c" /><br>

2.4. Under the Info column, search for the packet named ‘Client Hello’<br>
<img width="1919" height="1019" alt="Screenshot 2025-07-20 112212" src="https://github.com/user-attachments/assets/f92beaf1-d577-41cb-832a-042c0591a1ec" /> <br>

2.5. Copy and paste the destination IP address on the browser <br>
<img width="1919" height="969" alt="Screenshot 2025-07-20 112300" src="https://github.com/user-attachments/assets/1962d717-f3dc-4d35-ac50-7e5a5679bfea" /> <br>

2.6. The page will redirect to duckduckgo.com. This IP address will forward the request to the client website you visited earlier.<br>
<img width="1157" height="968" alt="Screenshot 2025-07-20 112546" src="https://github.com/user-attachments/assets/6737a464-0ab5-475d-bef4-cd93172fd546" /><br>














