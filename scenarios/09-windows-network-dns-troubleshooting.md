# Scenario 09 – Windows Network and DNS Troubleshooting

## Scenario

A simulated employee, John Smith, reported network connectivity problems on his Windows workstation.

The objective was to investigate network configuration, verify connectivity, reproduce a DNS timeout and demonstrate how to isolate the issue.

## Lab Environment

* Windows 11 Pro
* Microsoft Entra-joined workstation
* User: John Smith
* Virtualisation: UTM
* Network adapter: Red Hat VirtIO Ethernet Adapter

## Troubleshooting Process

### 1. Verify Network Configuration

Executed:

`ipconfig /all`

Identified the following configuration:

| Property        | Value         |
| --------------- | ------------- |
| IPv4 Address    | 192.168.64.2  |
| Subnet Mask     | 255.255.255.0 |
| Default Gateway | 192.168.64.1  |
| DHCP Server     | 192.168.64.1  |
| IPv4 DNS Server | 192.168.64.1  |

Confirmed that DHCP was enabled.

### 2. Test Default Gateway

Executed:

`ping 192.168.64.1`

Result:

* Four packets sent and received.
* 0% packet loss.
* Gateway connectivity successful.

### 3. Test External Connectivity

Executed:

`ping 1.1.1.1`

Result:

* Four packets received.
* 0% packet loss.
* Average latency: 13 ms.

Confirmed external IP connectivity.

### 4. Verify DNS Resolution

Executed:

`nslookup microsoft.com`

Successfully resolved the domain to IPv4 and IPv6 addresses.

### 5. Simulate DNS Failure

Executed:

`nslookup microsoft.com 192.0.2.1`

Result: DNS request timed out.

This deliberately queried an unavailable test DNS server without changing the workstation's actual network configuration.

### 6. Verify Working DNS Server

Executed:

`nslookup microsoft.com 192.168.64.1`

Result: DNS resolution successful.

The comparison demonstrated that the simulated timeout was specific to the unavailable DNS server.

## Outcome

Successfully verified the workstation's network configuration, gateway connectivity, external IP connectivity and DNS resolution.

Demonstrated how to isolate a simulated DNS failure by comparing responses from unavailable and functioning DNS servers.

No network configuration changes were required.

## Skills Demonstrated

* Windows network troubleshooting
* TCP/IP fundamentals
* DHCP configuration verification
* Default gateway testing
* DNS troubleshooting
* Command-line diagnostics
* Systematic fault isolation
* Service Desk technical documentation
