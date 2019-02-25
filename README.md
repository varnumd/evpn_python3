# Generate Ansible host_vars for EVPN lab

This Python3 script will take in these variables and generate the individual host_vars files for Ansible:

num_spines = 2
num_leafs = 8
p2p_range = '10.0.'
lo0_range = '10.0.250.'
lo1_range = '10.0.255.'
ibgp_range = p2p_range + str(num_spines+1) + '.'
ibgp_vlan = '4091'
asn_start = 65000

The script assumes that particular interfaces are used to connect leafs to spines, and leafs to leafs. 

If you want to change any of these parameters, just make the change directly in the script. 
