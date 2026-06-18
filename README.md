### GCP HA VPN process

- Make sure both GCP provider blocks and backends are set up and functional and in the same region. 

- Run terraform processes to initialize the provider and backend.

- Setup your VPC, subnets, and HA VPN. With the correct naming schemes, adequate subnets, and regions. Create these process for your networks section....
	- Two HA VPN gateway, two VPC network, two subnets for each VPC network, two routers, four tunnels, four router interfaces (two interfaces for router1/tunnel1-2 & two interfaces for router2/tunnel3-4), then four router peers (two peers for router1 & two peers for router 2). 

- Repeat this process for the other client as well. With different naming schemes. 
		Take note of all IP ranges, ASN's, regions, routers, peer IP address, and peer ASN.

- Run Terraform processes to see if all the code works correctly.

- Setup firewall rules to allow vpn traffic. udp 500 (icmp), 4500(esp) in both VPC's for each client.

- Make password keys for each tunnel and make sure they match both clients for peering
