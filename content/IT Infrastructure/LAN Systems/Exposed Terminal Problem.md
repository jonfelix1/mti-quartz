---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Exposed Terminal Problem

## Overview

- The **Exposed Terminal Problem** occurs in wireless networks when a device is unable to transmit data due to interference from another device that is transmitting to a different destination.
- This problem results in inefficient use of the network medium, as the exposed terminal unnecessarily defers its transmission.

## Example Scenario

- **Devices A and B** are within range of each other and communicating with **Device C** and **Device D**, respectively.
- If **Device A** wants to transmit data to **Device C**, but **Device B** is already transmitting to **Device D**, **Device A** might be unable to transmit even though **Device B**'s transmission does not interfere with **Device A**'s intended communication.

## Causes

- **Overhearing Transmissions**: **Device A** defers its transmission because it hears **Device B**'s transmission, even though it does not interfere with **Device A**'s communication with **Device C**.
- **Medium Reservation**: **Device A** is incorrectly prevented from using the medium due to the reservation made by **Device B** for its own communication.

## Impact

- **Inefficient Medium Utilization**: The network medium is underutilized because devices are unnecessarily prevented from transmitting data.
- **Reduced Throughput**: Overall network performance and throughput may be decreased due to the incorrect deferral of transmissions.

## Solutions

### Network Protocols

- **Network Protocol Enhancements**:
  - Use of protocols that better manage medium access and reduce the impact of the exposed terminal problem.
  - Implement mechanisms that allow devices to determine whether a transmission will actually cause interference.

### Carrier Sense Multiple Access with Collision Avoidance (CSMA/CA)

- **CSMA/CA Adjustments**:
  - Improve the CSMA/CA protocol to handle situations where transmissions are unnecessarily deferred.

### Directional Antennas

- **Directional Antennas**:
  - Use directional antennas to limit the transmission range and reduce interference with devices outside the intended communication area.

## Summary

- The **Exposed Terminal Problem** results from a device deferring its transmission due to perceived interference from a transmission that does not actually impact its communication.
- Solutions involve enhancing network protocols, adjusting CSMA/CA, and using directional antennas to improve medium utilization and network efficiency.


