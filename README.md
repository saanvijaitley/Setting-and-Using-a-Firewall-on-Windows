# Setting-and-Using-a-Firewall-on-Windows
# Windows Firewall Configuration – Block Telnet (Port 23)

#Objective
Block inbound traffic on port 23 (Telnet) using Windows Defender Firewall and confirm the rule works.
 Steps Taken
1. Opened **Windows Defender Firewall with Advanced Security**
2. Added a new **Inbound Rule**:
   - Type: Port
   - Protocol: TCP
   - Port: 23
   - Action: Block
3. Enabled **Telnet Client** using Windows Features
4. Tested with:
   -cmd
   -telnet localhost 23
Result: Connection failed, confirming port 23 is blocked.
