# CTI-Integration-Lab

## Objective

The CTI-Integration Lab integrates OpenCTI with Splunk and incorporates the OTX AlienVault connector to enhance threat detection, enriches and push data to enhanced incident response in real time. By leveraging structured threat intelligence data, this setup enriches Splunk's SIEM capabilities, enabling security teams to correlate, analyze, and respond to cyber threats more effectively.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in using Linux command-line tools e.g Docker-Compose.
- Ability to work extensively with command-line interfaces during the integration and configuration processes.
- hands-on experience in managing Linux environments, enhancing my technical skill set.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system to Invoke KV Store lookups.
- OPENCTI Developed & maintained by the Filigran team.
- OpenCTI External Connectors (OTX AlienVault)
- 2 UBUNTU SERVER (opencti) (splunk)

### Example Use Case

Imagine you're monitoring network traffic in Splunk, and OpenCTI has identified a malicious IP address linked to a known threat actor. With the integration in place:

The IP address is automatically ingested into Splunk from OpenCTI.
When the malicious IP is detected in network traffic logs, Splunk generates an alert.
Analysts can view detailed information about the threat actor, including associated TTPs, in the same dashboard, enabling a more efficient and informed response.

## Steps

*Ref 1: Install Docker Compose, as it will be used to deploy and manage the OpenCTI environment*

<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/docker-compose%20install%201.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/docker%20install2.png" />

*Ref 2: Clone the OpenCTI repository from GitHub*

<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/gthub%20clone%20OpenCTI%20docker.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/gthub%20clone%20OpenCTI%20docker.png" />

*Ref 3: Rename the .env.sample file to .env*

<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/rename%20.env%20sample%20to%20.env.png" />

*Ref 4: Generate a UUID for the admin token and update the password for Web GUI access to OpenCTI*

<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/Config%20.env%20and%20editing.png" />

*Ref 5: Access to OpenCTI GUI and log in using the admin credentials.*

<img src="https://github.com/mullarcyber/CTI-images/blob/76b634c040f3edc5060c0479afd4f6acde79bbfe/opencti%20GIU%20login.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/76b634c040f3edc5060c0479afd4f6acde79bbfe/opencti%20GIU.png" />

*Ref 6: AlienVault connector has been updated, and data is now being pushed to OpenCTI*

<img src="https://github.com/mullarcyber/CTI-images/blob/82db37d0f8beecc78cca6795896d6546b27f3c9f/allienVault%20connector.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/82db37d0f8beecc78cca6795896d6546b27f3c9f/allienvault%20pulling%20data%20in.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/33d717e4a3fe416bd591a2e6a9957fa479ce14ec/cti%20allien%20vault%20data.png" />

*Ref 7: Splunk token connector has been updated and is now configured to receive data from CTI.*

<img src="https://github.com/mullarcyber/CTI-images/blob/14117ba6e0ca186bc4c1ba2dcdf1469e55aac434/splunkconnectorupdated.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/14117ba6e0ca186bc4c1ba2dcdf1469e55aac434/splunk%20connected%20with%20cti.png" />

*Ref 8: Splunk KV Store has been created to enhance threat visualization and enable swift action using contextual data from OpenCTI.*

<img src="https://github.com/mullarcyber/CTI-images/blob/64cabb885f97d0dceb7af88443fa1f89d0274ca4/KV%20Store.png" />
<img src="https://github.com/mullarcyber/CTI-images/blob/64cabb885f97d0dceb7af88443fa1f89d0274ca4/realtime%20visualization.png" />

### Summary and Conclusion

OpenCTI-Splunk integration enhances cybersecurity operations by combining real-time threat intelligence with advanced logging and analysis capabilities. It improves threat visibility by enriching security events with detailed context, enabling faster response and more informed decision-making. Analysts gain a proactive defense advantage through early detection of threat actors and updated IoCs and TTPs from OpenCTI.
This integration streamlines threat management, empowering analysts to access critical information within a single tool, ensuring efficient and effective protection of the environment.







