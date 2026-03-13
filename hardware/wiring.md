\# Wiring Guide



\## ESP32 to Relay Module

| ESP32 Pin | Relay Pin |

|-----------|-----------|

| GPIO 26   | IN1       |

| 3.3V      | VCC       |

| GND       | GND       |



\## ESP32 to PZEM-004T

| ESP32 Pin | PZEM Pin  |

|-----------|-----------|

| GPIO 16 (RX) | TX    |

| GPIO 17 (TX) | RX    |

| 5V        | VCC       |

| GND       | GND       |



\## ESP32 to DHT22

| ESP32 Pin | DHT22 Pin |

|-----------|-----------|

| GPIO 4    | DATA      |

| 3.3V      | VCC       |

| GND       | GND       |



\## Power Supply (Hi-Link HLK-PM01)

| HLK-PM01  | Connects To |

|-----------|-------------|

| L         | AC Live     |

| N         | AC Neutral  |

| +5V       | ESP32 VIN   |

| GND       | Common GND  |

