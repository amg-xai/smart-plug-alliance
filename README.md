# Smart Plug Alliance 🔌
A sustainable, voice-controlled smart plug built with ESP32.
Supports Alexa & Siri via Matter protocol.

## Team
GreenPlug Guardians

## Status
🚧 Work in progress — Hardware acquired, firmware ready, building prototype next.

---

## Project Overview
A smart plug that allows remote control of appliances via mobile app, schedules, 
and voice assistants (Alexa & Siri). Plugs into any wall socket and controls 
devices like fans, lights, and ACs.

---

## Features
- ✅ ON/OFF control via voice (Alexa & Siri)
- ✅ Energy monitoring (voltage, current, power, frequency)
- ✅ Temperature & humidity automation via DHT22
- ✅ Physical manual button on the plug
- ✅ Overload protection (auto cut-off above 3000W)
- ✅ OTA (Over-the-Air) firmware updates
- ✅ Low standby power (<0.5W using ESP32 deep sleep)
- ✅ Works locally without internet (Home Assistant)
- ✅ Cross-platform via Matter protocol

---

## Tech Stack
| Layer | Technology |
|-------|------------|
| Microcontroller | ESP32 (S3/C3) |
| Firmware | ESPHome (YAML) |
| Hub | Home Assistant |
| Protocol | Matter (Alexa, Siri, Google Home) |
| Communication | MQTT |
| Dev Tools | VS Code, ESPHome Web Flasher |
| Cloud (optional) | Home Assistant Cloud |

---

## Hardware Components
| Component | Purpose | Quantity |
|-----------|---------|----------|
| ESP32 Dev Board (S3/C3) | Microcontroller | 1 |
| 16A Relay Module | ON/OFF control | 1-4 |
| PZEM-004T v3 | Energy monitoring | 1 |
| DHT22 Sensor | Temperature & humidity | 1 |
| Hi-Link HLK-PM01 | Power supply | 1 |
| Fuse | Safety protection | 1 |
| Varistor | Surge protection | 1 |
| Enclosure (3D Printed) | Housing | 1 |

---

## Wiring
See [hardware/wiring.md](hardware/wiring.md) for full pin connections.

### Quick Reference
- ESP32 GPIO26 → Relay IN1
- ESP32 GPIO16/17 → PZEM-004T (UART)
- ESP32 GPIO4 → DHT22 DATA
- ESP32 GPIO0 → Manual Button
- ESP32 GPIO2 → Status LED

---

## Firmware
See [firmware/smart-plug.yaml](firmware/smart-plug.yaml) for full ESPHome config.

### Before Flashing
Edit these two lines in the YAML file:
```yaml
ssid: "YOUR_WIFI_NAME"
password: "YOUR_WIFI_PASSWORD"
```

---

## Cost
| Item | Cost |
|------|------|
| Total Prototype | ₹1,500 - ₹2,200 |
| Software | Free (open-source) |
| vs Commercial Plugs | ₹2,500+ for similar features |

Energy savings pay back cost in **6-12 months**.

---

## Sustainability
- Low standby power (<0.5W)
- Recycled plastic enclosure
- RoHS-compliant PCBs
- OTA updates (no hardware waste)
- Vampire power detection
- CO2 savings tracker
- Solar compatible (optional DC input)
- Helps save 10-20% on electricity bills

---

## Safety
- 230V AC — fuses and isolation used
- Overload protection (auto cut-off)
- Child lock feature
- BIS (India) & RoHS certification planned

---

## Future Scope
- AI predictive automations via Edge ML
- Solar panel & smart grid integration
- Mobile app development
- Research publication on energy savings

---

## Roadmap
- [x] Project concept & ideation
- [x] Hardware acquired
- [x] Firmware written (ESPHome)
- [x] Wiring diagram documented
- [ ] Breadboard prototype build
- [ ] Home Assistant integration
- [ ] Voice control testing
- [ ] PCB design
- [ ] Enclosure 3D print
- [ ] Safety testing & certifications
