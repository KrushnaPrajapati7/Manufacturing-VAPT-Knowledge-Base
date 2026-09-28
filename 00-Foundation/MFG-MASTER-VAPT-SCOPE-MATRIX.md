# Master VAPT Scope Matrix

**Y** = commonly applicable. **Context** = depends on implementation. **N/A** = normally outside direct focus.

| Asset Family | Asset / Technology | Recon | Scan | Vuln | Identity | App/API | OT/ICS | Impact | Report | Safety |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---|
|External / Internet-Facing|domains|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|subdomains|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|DNS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|public IPs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|internet gateways|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|edge routers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|firewalls|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|WAF|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|load balancers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|reverse proxies|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|CDN|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|API gateways|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|web applications|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|admin panels|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|cPanel/hosting panels|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|webmail|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|customer portals|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|supplier portals|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|RFQ portals|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|authentication portals|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|VPN gateways|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|External / Internet-Facing|remote-access portals|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|public cloud endpoints|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|External / Internet-Facing|public storage|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|Windows servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|Linux servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|application servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|web servers|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Corporate IT|database servers|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Corporate IT|file servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|backup servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|DNS/DHCP/NTP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|Active Directory|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|Domain Controllers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|LDAP|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|Entra ID/IdP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|SSO|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|MFA infrastructure|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|PKI/certificate authorities|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|PAM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|endpoints|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|engineering laptops|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|thin clients|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|mobile devices|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|printers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|scanners|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|NAS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|SAN|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|VMware|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|Hyper-V|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|KVM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|management servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Corporate IT|patch-management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|software-deployment|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Corporate IT|MDM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|ERP|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|SAP|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|SAP HANA|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|Oracle ERP|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|Dynamics|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|CRM|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|HRMS|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|finance systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|procurement systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|supply-chain systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|document management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|collaboration|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|email|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Enterprise & Business Applications|Microsoft 365/Google Workspace|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|MES|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Manufacturing Operations|MOM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|QMS|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Manufacturing Operations|WMS|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Manufacturing Operations|CMMS|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Manufacturing Operations|LIMS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|SCM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|production scheduling|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|OEE|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|traceability|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|work instructions|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|recipe management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|quality inspection|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|maintenance systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|electronic batch records|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Manufacturing Operations|production dashboards|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|CAD|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Engineering & IP|CAM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|CAE|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|PLM|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Engineering & IP|PDM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|engineering workstations|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|CNC programming|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|PLC programming|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Engineering & IP|design repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|CAD repositories|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Engineering & IP|BOM repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|technical drawings|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|product specifications|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|firmware repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|source-code repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|R&D systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Engineering & IP|simulation systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|OT / ICS|SCADA|Y|Y|Y|Y|Y|Y|Y|Y|Restricted|
|OT / ICS|SCADA servers|Y|Y|Y|Y|Y|Y|Y|Y|Restricted|
|OT / ICS|SCADA clients|Y|Y|Y|Y|Y|Y|Y|Y|Restricted|
|OT / ICS|DCS|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|DCS servers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|PLC|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|PAC|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|RTU|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|HMI|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|historian|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|alarm servers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|event servers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|engineering stations|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|control servers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|application servers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|OT / ICS|data gateways|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|industrial PCs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|safety controllers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|OT / ICS|industrial gateways|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|CNC machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|industrial robots|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|robot controllers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|AGVs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|AMRs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|assembly machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|welding systems|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|cutting machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|press machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|packaging machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|inspection machines|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|machine vision|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|3D printers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|conveyors|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|automated storage|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|test equipment|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|calibration equipment|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|machine tools|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial / Cyber-Physical|process equipment|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|sensors|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|actuators|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|motors|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|valves|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|drives|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|VFDs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|servo drives|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|relays|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|contactors|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|smart instruments|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|IEDs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|remote I/O|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|Field Devices & Instrumentation|industrial meters|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|industrial Ethernet|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|managed switches|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|industrial switches|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|routers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|industrial routers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|industrial firewalls|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|wireless bridges|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|network taps|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|Modbus|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|Modbus TCP|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|OPC UA|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|EtherNet/IP|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|PROFINET|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|DNP3|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|MQTT|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|AMQP|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|HART|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|CAN-related protocols|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|serial protocols|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Industrial Networks & Protocols|vendor protocols|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|smart sensors|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|IIoT gateways|Y|Y|Y|Context|Y|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|edge computers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|industrial PCs|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|device-management platforms|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|machine-monitoring platforms|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|IoT APIs|Y|Y|Y|Y|Y|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|MQTT brokers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|OPC gateways|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|remote diagnostics|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|predictive maintenance|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|digital twins|Y|Y|Y|Context|Y|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|industrial analytics|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|IIoT / Edge / Industry 4.0|data platforms|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Cloud & Digital Infrastructure|AWS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|Azure|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|GCP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|private cloud|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|hybrid cloud|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|VMs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|containers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|Kubernetes|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|registries|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|serverless|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|object storage|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|S3|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|Azure Blob|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|cloud databases|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|data lakes|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|data warehouses|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|VPC/VNet|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|subnets|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|security groups|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|NACLs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|load balancers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|API gateways|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|IAM|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|service accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|secrets|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|cloud keys|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Cloud & Digital Infrastructure|private endpoints|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|REST|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|SOAP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|GraphQL|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|WebSockets|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|gRPC|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|vendor APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|cloud APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|mobile APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|ERP APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|MES APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|PLM APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|IoT APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|webhooks|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|ESB|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|message brokers|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|API & Integration|ETL pipelines|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|event buses|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|SFTP/file integrations|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|API & Integration|middleware|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|SSL VPN|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|IPsec VPN|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|site-to-site VPN|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|vendor VPN|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|RDP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|SSH|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|VNC|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|jump servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|bastions|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|remote support platforms|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|vendor maintenance|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|MSPs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|MSSPs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|system integrators|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|equipment vendors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|software vendors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|maintenance contractors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|remote engineering|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|third-party APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Remote Access & Third Parties|software update channels|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|PII|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|employee data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|customer data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|supplier data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|financial data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|production data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|quality data|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|machine telemetry|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|process parameters|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|recipes|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|CAD/IP|Y|Context|Y|Y|Y|N/A|Y|Y|Controlled|
|Data & Information|drawings|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|BOM|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|source code|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|firmware|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|credentials|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|API keys|Y|Context|Y|Y|Y|N/A|Y|Y|Controlled|
|Data & Information|tokens|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|certificates|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|private keys|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|configuration files|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Data & Information|backups|Y|Context|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|backup servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Backup / DR|backup repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|offline backups|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|immutable backups|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|cloud backups|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Backup / DR|replication|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|snapshots|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|database backups|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Backup / DR|PLC backups|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Backup / DR|SCADA backups|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Backup / DR|HMI backups|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Backup / DR|engineering backups|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Backup / DR|disaster-recovery systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|SIEM|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|SOAR|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|EDR|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|XDR|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|IDS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|IPS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|NDR|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|vulnerability management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|patch management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|OT IDS|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|OT network monitoring|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|asset discovery|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|log servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Security Monitoring|Windows logs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|firewall logs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|VPN logs|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Security Monitoring|application logs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Security Monitoring|API logs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Security Monitoring|cloud logs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Security Monitoring|SCADA logs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Security Monitoring|HMI logs|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Security Monitoring|authentication logs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|corporate Wi-Fi|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|industrial Wi-Fi|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|wireless sensors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|Bluetooth|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|BLE|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|RFID|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|NFC|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|wireless controllers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|tablets|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|rugged tablets|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|barcode scanners|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|RFID readers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|mobile printers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|forklift terminals|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Wireless / Mobile|mobile manufacturing applications|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Physical / Facility / Safety|CCTV|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|NVR|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|DVR|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|access control|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|badge readers|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|biometrics|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|turnstiles|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|visitor management|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|BMS|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|HVAC|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|lighting control|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|fire alarm systems|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|power monitoring|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|UPS|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|generators|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|environmental monitoring|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|safety PLC|Y|Y|Y|Y|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|safety controllers|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|emergency stops|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|safety interlocks|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Physical / Facility / Safety|fire/gas systems|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Software Supply Chain / DevSecOps|Git|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|GitHub|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|GitLab|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|Bitbucket|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|Jenkins|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|CI/CD|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|build servers|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|artifact repositories|Y|Y|Y|Context|Y|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|container registries|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|package repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|dependency management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|code signing|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|secrets management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|Infrastructure-as-Code|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Software Supply Chain / DevSecOps|configuration repositories|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|employees|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|operators|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|engineers|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|IT admins|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|OT admins|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|domain admins|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|application admins|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|DBAs|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|vendors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|contractors|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|service accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|machine accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|API identities|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Identity & Privilege|cloud identities|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|Identity & Privilege|break-glass accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|shared accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Identity & Privilege|dormant accounts|Y|Y|Y|Y|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|TLS certificates|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|internal certificates|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|PKI|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|device certificates|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|code-signing certificates|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|key-management|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|NTP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|PTP|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|GPS time|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Cryptographic / Time Services|industrial time synchronization|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|Plant Utilities|electrical systems|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|smart meters|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|compressed air|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|steam|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|water|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|cooling|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|HVAC|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|energy management|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|Plant Utilities|utility monitoring|Y|Y|Y|Context|Context|Y|Y|Y|Restricted|
|AI / Analytics|AI/ML platforms|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|predictive maintenance|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|computer vision|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|ML pipelines|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|analytics platforms|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|data science platforms|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|AI APIs|Y|Y|Y|Y|Y|N/A|Y|Y|Controlled|
|AI / Analytics|model serving|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
|AI / Analytics|generative AI systems|Y|Y|Y|Context|Context|N/A|Y|Y|Controlled|
