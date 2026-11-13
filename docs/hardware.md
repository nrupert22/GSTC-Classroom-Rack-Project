```                                          
   ┌───────────────────────────────────┐  
   │ ┌───────────────────────────────┐ │  
   │ │ ┌───────┐  ┌───────┐ ┌──────┐ │ │  
   │ │ │ CORE  │  │ CORE  │ │  L3  │ │ │  
   │ │ │  01   │  │  02   │ │ CACHE│ │ │  
   │ │ │       │  │       │ │      │ │ │  
   │ │ └───────┘  └───────┘ │      │ │ │  
   │ │ ┌───────┐  ┌───────┐ │      │ │ │  
   │ │ │ CORE  │  │ CORE  │ └──────┘ │ │  
   │ │ │  03   │  │  04   │          │ │  
   │ │ │       │  │       │          │ │  
   │ │ └───────┘  └───────┘          │ │  
   │ │                               │ │  
   │ └───────────────────────────────┘ │  
   └───────────────────────────────────┘  
  ```
# Server Hardware and Sub-components
```text
| Hostname: 
| Model: Dell Poweredge R610 
| Manufacture Date:
| CPU: 2x Intel Xeon X5550 (16) @2.67 GHz
| Cores/Threads: 4/8 per chip for total of 8/16 combined
| RAM Total: 12GB
| RAM Stick x GB:
| RAM Speed: 1333Mhz
| ECC: Yes
| Storage: 2x 300GB SAS (Raid 1 boot)  
| PCIE: Nework card (Unused)
| Purpose/OS: Routing & Firewall/OPNSense

| Hostname: Installation-02
| Model: Dell Poweredge R730
| Manufacture Date:
| CPU: 2x Intel(R) Xeon(R) E5-2630 V3 (32) @3.20 Ghz 
| Cores/Threads: 8/16 per chip for total of 16/32 combined
| RAM Total: 192 GB
| RAM Stick x GB:   
| RAM Speed: 2133Mhz
| ECC: Yes
| Storage: 3x 146GB SAS (Raid Z1 boot), 2x 250GB SSD (Raid 1), 7x 1TB SAS (ZFS?)  
| PCIE:  
| Purpose/OS: VMs & LXC/Proxmox

| Hostname: Installation-03
| Model: Dell Poweredge R640
| Manufacture Date:
| CPU: 2x Intel(R) Xeon(R) Silver 4215 (32) @3.20 Ghz  
| Cores/Threads: 8/16 per chip for total of 16/32 combined
| RAM Total: 128GB
| RAM Stick x GB: 16x8GB
| RAM Speed:  
| ECC: Yes
| Storage: 
| PCIE:  
| Purpose/OS: VMs & LXC/Proxmox

| Hostname: Installation-04
| Model: Dell Poweredge R730
| Manufacture Date:
| CPU:  
| Cores/Threads:   
| RAM Total:  
| RAM Stick x GB:   
| RAM Speed:  
| ECC:  
| Storage: 1x 480GB SSD (Boot), 3x 2TB HDD (Raid Z1), 4x 4TB HDD (Raid Z2)
| PCIE:  
| Purpose/OS: Proxmox/Mass Datastorage

| Hostname: Installation-05
| Model: Dell Poweredge R730
| Manufacture Date:
| CPU:  
| Cores/Threads:   
| RAM Total:  
| RAM Stick x GB:   
| RAM Speed:  
| ECC:  
| Storage:  
| PCIE:  
| Purpose/OS:


  ```
