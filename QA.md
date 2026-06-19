Individual work Q&A

Explain the differences and similarites between HA VPN and NCC.

Similarities:

NCC (Network Connectivity Center) is a framework in GCP that centralizes how businesses or enterprises connect global networks.
An example is that it uses hub-and-spoke model to unify VPC's. 

HA VPN (High availability) cloud VPN is a GCP service that allows you to secure and connect your on premises networks or other clouds to your GCP network via IPsec VPN

Differences:

They use different topologies, HA VPN uses point to point access from your own networks or between local networks. 
NCC uses Hub-and-spoke to access multiple networks.

Explain the use cases of HA VPN vs NCC?

HAVPN: Low cost local cloud conntectivity on premises or partner to partner. 
NCC: Used for enterprises or businesses for centralized routing. Multi-VPC, multi-hub, multi-cloud, etc.

Explain the use cases of the NIC (Network Intelligence Center).

One use case is connectivity tests verifies if a source can reach a destination and pinpoint where and why it failed
Another use case is Flow Analyzer. FA will analyze VPC flow logs quick and efficiently without much hassle. Also lets you perform opinionated network traffic analysis to optimize for security, complience, performance, and cost.
Firewall insights is another use case. FI provides data about how firewall rules are used, exposes misconfigs, and identifies rules that can be more strict.




https://cloud.google.com/network-intelligence-center
https://docs.cloud.google.com/network-connectivity/docs/network-connectivity-center/concepts/overview
https://docs.cloud.google.com/network-connectivity/docs/vpn/concepts/overview
https://docs.cloud.google.com/network-intelligence-center/docs/overview
