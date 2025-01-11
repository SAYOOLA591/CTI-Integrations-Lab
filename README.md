# CTI-Integrations-Lab

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

*Ref 4: Generate a UUID for the admin token and update the password for Web GUI access in OpenCTI*

<img src="https://github.com/mullarcyber/CTI-images/blob/79569250e3273659fb10a024bdfc7ce4afddf1a7/Config%20.env%20and%20editing.png" />





