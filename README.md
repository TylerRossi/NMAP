# NMAP

**Red Team**
	Syn scan is stealth. Can bypass IDS and no log event created for a connection not fully established. need sudo premission
	firewall evasion
		run a -sX: christmas tree scan
	bypass ping first as this is usually blocked: -Pn
	
**Blue Team**
	ping sweep to enumerate: -sn
  how to defend
	configure a firewall to respond with a RST TCP packet.
		iptables -I INPUT -p tcp --dport <port> -j REJECT --reject-with tcp-reset

