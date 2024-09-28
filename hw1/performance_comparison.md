
# Performance Comparison

1. **Latency (us)**
   - Local DRAM has the lowest latency (0.1122 us), making it the fastest in terms of access speed.
   - Rack DRAM has relatively higher latency (240.1122 us) compared to Local DRAM, but it’s still faster than Local Disk and Rack Disk.
   - Local Disk and Rack Disk have significantly higher latencies (368.4 us and 608.4 us respectively), indicating they are slower to access.
   - To find the latency for the rack, we combine the network communication latency (the time it takes to transfer data over the network to the rack) with the local latency (the time it takes to access the storage or memory within the rack). This sum gives the total latency for accessing resources in the rack.

2. **Bandwidth (MB/s)**
   - Local DRAM offers the highest bandwidth (120364.2 MB/s), meaning it can handle a larger amount of data being transferred per second.
   - To determine the bandwidth for rack disk, we take the lowest bandwidth from the components involved in the data path because the bottleneck restricts overall performance.

3. **Capacity (KB)**
   - Rack Disk has the highest capacity (19204120 KB), showing that it can store the most data.
   - Local Disk (480103 KB) and Local DRAM (131489.08 KB) have much lower capacities compared to the options in the rack, but Local DRAM sacrifices capacity for high speed.
