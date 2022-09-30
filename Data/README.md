# Data - RAW `pcap` Files (Network Capture)
> It was performed using an external network interface on monitor mode.

# Available files
> It was used a filter before exporting the pcap files to remove all data over TCP, the filter command from Wireshark was the `not tcp`. This change reduced more the `Flight` related data, data normally contains image captured by the Parrot AR.Drone and transmitted over TCP.

```
Data/
├── Attack
│   ├── De-Authentication
│   ├── DoS_Hping
│   └── UDP Flood
└── Normal
    ├── Establishing_connection
    ├── Flights
    └── Takeoff_and_landing
```

The available `pcap` files are available compressed with GZip. They are separated on two major classes `Attack` containing the performed attacks, and `Normal` that represents network traffic from three scenarios: Establishing a controller to UAV connection (`Establishing_connection`), random flights performed (`Flights`), and commands of Takeoff and Landing (`Takeoff_and_landing`).

## MAC Address for Interpreting Traffic
- Parrot AR.Drone MAC Address: `90:03:B7:38:F5:B8`
- Laptop MAC Address: `0C:84:DC:D5:5F:4D`
- Mobile Phone MAC Address (UAV Remote Controller): `44:80:EB:00:0B:41`

