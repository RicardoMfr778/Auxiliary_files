Replace xadapter.c file on the lwip v1.1.8 library by the one in this folder.

In alternative, find the xemac_add function on line 123 and add a break statement at the end of each case statement:
	- "case xemac_type_xps_emaclite"
	- "case xemac_type_axi_ethernet"

This prevents the ping system from failing to determine the type of EMAC of the given address.