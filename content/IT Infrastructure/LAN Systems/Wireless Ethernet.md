---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Wireless Ethernet

## Overview

- **Wireless Ethernet** (also called [[Wi-Fi]]) allows **workstations** to connect to a network as long as they are within the range of an **access point**.
- Various versions of the **IEEE 802.11 standard** define different wireless LAN connections.
- Collisions for communication is done using [[Wireless CSMA CA]] 
- Some problems of wireless ethernet are [[Hidden Terminal Problem]] and [[Exposed Terminal Problem]]
- [[WLAN Frequency Planning]] is used to manage radio waves.
- 

## Basic Components

- **Client Radio**: Typically a **PC card** with an integrated antenna, installed in laptops or workstations.
- **Access Point (AP)**: Contains an Ethernet port and a transceiver. The AP acts as a bridge between **wired** and **wireless networks** and can perform basic **routing functions**.

## Service Sets

- **Basic Service Set (BSS)**: Workstations with client radio cards within the range of a single access point.
- **Extended Service Set (ESS)**: Multiple Basic Service Sets interconnected to form a larger network.

## Frequency Bands

- **ISM Band**: Includes 900 MHz, 2.4 GHz, and 5 GHz frequencies used for wireless communication.

## IEEE 802.11 Standards

| Standard      | Release Year | Maximum Data Rate | Frequency Bands | Description |
|---------------|--------------|-------------------|-----------------|-------------|
| **802.11**    | 1997         | 2 Mbps            | 2.4 GHz         | The original wireless standard. |
| **802.11b**   | 1999         | 11 Mbps           | 2.4 GHz         | Known as Wi-Fi. Improved data rate over 802.11. With directional antennas, can reach up to 16 km; typically 100 feet (30 m) with omni-directional antennas. |
| **802.11a**   | 2002         | 54 Mbps           | 5 GHz           | Faster standard with a higher frequency, providing less interference. Max transmission distance of 90 feet (27 m). |
| **802.11g**   | 2002         | 54 Mbps           | 2.4 GHz         | Operates on the same frequency as 802.11b but with higher data rates. Backwards compatible with 802.11b. |
| **802.11n**   | 2009         | 600 Mbps (theoretical) | 2.4 GHz, 5 GHz | Uses MIMO technology for higher data rates and improved reception. Actual data rates range from 100 to 145 Mbps. |
| **802.11ac**  | 2013         | 1.3 Gbps (theoretical) | 5 GHz           | Also known as Wi-Fi 5. Supports wider channels and higher data rates with improved MIMO technology. |
| **802.11ax**  | 2019         | 9.6 Gbps (theoretical) | 2.4 GHz, 5 GHz, 6 GHz | Known as Wi-Fi 6. Introduces higher data rates, improved efficiency, and better performance in dense environments. Supports the 6 GHz band in addition to 2.4 GHz and 5 GHz. |

## Summary

- **IEEE 802.11** standards have evolved from basic data rates and limited frequency bands to advanced technologies offering higher data rates, improved efficiency, and greater coverage.
- **Wi-Fi 6 (802.11ax)** represents the latest advancement, enhancing performance and efficiency, especially in crowded network environments.


