<p align="center">
  <img src="https://github.com/user-attachments/assets/a9e62984-6877-41d3-b24c-25d0460b9005" alt="Microsoft Azure Banner">
</p>

<h1>Testing VPN and IP Address Differences in Azure VMs</h1>

<p>In this lab, I set up a Virtual Machine (VM) in Azure, used ProtonVPN to test VPN connections, and analyzed how the IP addresses and website behaviors change based on different geographic locations.</p>

<h2>Part 1: Create a Virtual Machine in Azure</h2>

<p><strong>Step 1: Note Your Current IP Address</strong></p>
<ul>
  <li>First, from within my actual computer, I browsed to <a href="https://whatismyipaddress.com/" target="_blank">https://whatismyipaddress.com/</a> to take note of my current IP address. I saved this information in a text file for later comparison.</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a519dbc6-ac93-4dd1-b44f-93eeb10849b7" alt="Step 1: Note Your Current IP Address" width="80%">
</p>



<p><strong>Step 2: Create a Resource Group and Virtual Machine</strong></p>
<ul>
  <li>Next, I logged into the <a href="https://portal.azure.com/">Azure Portal</a> and created a new Resource Group to organize the resources for this lab.</li>
  <li>After creating the Resource Group, I deployed a Windows 10 Virtual Machine </li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/6b7acb3f-2da0-4035-936b-47d8b37f097b" alt="Step 2: Create a Resource Group and Virtual Machine" width="80%">
</p>



<p><strong>Step 3: Log into the VM</strong></p>
<ul>
  <li>Once the VM was deployed, I connected to it using Remote Desktop and logged in with the credentials I set during the VM creation process.</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/1cfdccf1-875a-47f4-b258-7f3e91f6dcef" alt="Step 3: Log into the VM" width="80%">
</p>






<p><strong>Step 4: Note the VM's IP Address</strong></p>
<ul>
  <li>From within the VM, I browsed to <a href="https://whatismyipaddress.com/" target="_blank">https://whatismyipaddress.com/</a> and recorded the new IP address in my text file for comparison. The IP address was different from my actual computer's IP because the VM was in a different geographic location.</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/2bed0e5c-908a-47df-bed5-78e860d3f9ed" alt="Step 4: Note the VM's IP Address" width="80%">
</p>




<h2>Part 2: Sign Up for ProtonVPN and Test the VPN Connection</h2>

<p><strong>Step 5: Sign Up for ProtonVPN</strong></p>
<ul>
  <li>On my actual computer, I signed up for the free version of ProtonVPN at <a href="https://account.protonvpn.com/signup?plan=free&language=en" target="_blank">https://account.protonvpn.com/signup?plan=free&language=en</a>.</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/c999bd37-146f-4715-95ee-79ee19ef796a" alt="Step 5: Sign Up for ProtonVPN" width="80%">
</p>




<p><strong>Step 6: Download and Install ProtonVPN Client on the VM</strong></p>
<ul>
  <li>Within the VM, I downloaded the ProtonVPN client from the official website.</li>
  <li>Once installed, I logged into ProtonVPN using the credentials I created earlier.</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/542b79f6-b19d-4663-b114-ba1645b9ba04" alt="Step 6: Download and Install ProtonVPN Client" width="80%">
</p>



<p><strong>Step 7: Connect to a VPN Server in a Different Country</strong></p>
<ul>
  <li>After logging into ProtonVPN, I connected to a VPN server using quick connect.(Poland)</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f77474d1-0c60-4185-b222-e103ae754f93" alt="Step 7: Connect to a VPN Server in a Different Country" width="80%">
</p>



<p><strong>Step 8: Test the VPN Connection</strong></p>
<ul>
  <li>While still in the VM, I browsed to <a href="https://whatismyipaddress.com/" target="_blank">https://whatismyipaddress.com/</a> again. The IP address was now different from both my actual machine's IP and the original IP of the VM, showing that the VPN was successfully masking my location.</li>
  <li>I then browsed to websites like Google, Disney, and Amazon. I observed that the language or URLs sometimes changed to reflect the VPN server's location (e.g., google.co.pl for Poland).</li>
</ul>

<p align="center">
  <img src="https://github.com/user-attachments/assets/22de2be1-3c8f-414a-832f-74ed3dab3883" alt="Step 8: Test the VPN Connection" width="80%">
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/2371721b-66a6-46a0-b2c4-4d7ddf99acc8" alt="Step 8: Test the VPN Connection" width="80%">
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/79e80a91-1d54-4034-a4c5-253eab93ae6f" alt="Step 8: Test the VPN Connection" width="80%">
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/191a21f3-3844-4abc-8120-3a8fda68f797" alt="Step 8: Test the VPN Connection" width="80%">
</p>






<h2>Conclusion</h2>
<p>In this lab, I successfully created a Virtual Machine in Azure, tested VPN connections using ProtonVPN, and observed how IP addresses and website behaviors changed based on different geographic locations. This hands-on experience helped me understand the impact of VPNs and geographic locations on network configurations and website accessibility.</p>
