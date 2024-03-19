# Azure-Sentinel-Honeypot-SIEM

## Summary
In this project, I set up a virtual machine on Azure with a publically routable IP address and configure the firewalls to allow hackers from anywhere to attempt to log in. Then, I use a Geolocation.io API Key with a powershell script to extract the IP addresses of hackers and display them on a Sentiel world map.

## Technologies Used

- Azure
  - Virtual Machine
  - Log Analytics
  - Security Center
  - Sentinel
- Windows Defender Firewall
- Powershell
- Event Viewer
- [ipgeolocation.io](https://ipgeolocation.io/) API key

## Project Walk-through
 1. Create Azure Subscription
 2. Create Virtual Machine
 3. Firewall turn off / allow all in firewall
 4. Create Log Analytics Workspace
 5. Enable gathering VM logs in Security Center
 6. Connect Log Analytics to VM
 7. Setup Azure Sentinel
 8. Log into VM with Remote Desktop
 9. Observe Event viewer Logs in VM
 10. Turn off Windows Firewall on VM
 11. Running a powershell script
 12. Get Geolocation.io API Key 13 Run Script To get Geo Data from attackers
 13. Create custom log in LAW to bring in our custom log
 14. Create custom fields/extract fields from raw custom log data
 15. Testing Extracts
 16. Setup map in sentinel with Latitude and Longitude (or country)
 17. Fixing Map plot sizes
 18. Final check on map
