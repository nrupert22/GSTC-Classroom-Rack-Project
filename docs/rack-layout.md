                                          
   ┌───────────────────────────────────┐  
   │┌─────────────────────────────────┐│  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││┌┌──┐───────────────────────────┐││  
   ││││  │                           │││  
   ││└└──┘───────────────────────────┘││  
   ││                                 ││  
   ││                                 ││  
   │└─────────────────────────────────┘│  
   └───────────────────────────────────┘  
   
# Rack Devices (from top to bottom)
| Model: Aruba 2930M Switch
| Running: Aruba latest firmware
| Purpose: Layer 2 forwarding and segmentation
| Location: Top, reverse mounted

| Model: UniFi Access Point
| Purpose: SSID Broadcast and wireless access
| Location: Top, on top of R610

| Model: Dell Poweredge R610
| Running: OPNSense
| Purpose: Layer 3 Routing & Firewall
| Location: Top

| Model: 3x Dell Monitor with KVM
| Purpose: Dashboard display for Homarr, Weatherstar, and server direct access
| Location: Middle

| Model: 2x Dell Wysebox
| Running: Debian 13
| Purpose: Dashboard client for Homarr and Weatherstar
| Location: Middle

| Hostname: Installation-02
| Model: Dell Poweredge R730
| Running: Proxmox
| Purpose: Virtual Machines and Containers
| Location: Middle

| Hostname: Installation-03
| Model: Dell Poweredge R640
| Running: Proxmox
| Purpose: Virtual Machines and Containers
| Location: Middle

| Hostname: Installation-04
| Model: Dell Poweredge R730
| Running: 
| Purpose: Bulk Storage
| Location: Middle

| Hostname: Installation-05
| Model: Dell Poweredge R730
| Running: 
| Purpose: Bulk Storage
| Location: Middle

| Hostname: Installation-06
| Model: Dell Poweredge T620
| Running: 
| Purpose: 
| Location: Middle

| Hostname: MilkMilk
| Model: Dell Wysebox
| Running: Debian 13 and NUT-Server
| Purpose: UPS Monitoring, graceful shutdown, and serial aggregation
| Location: Bottom

| Model: 3x APC UPS Pro 1500
| Purpose: Surge protection and battery backup
| Location: Bottom
