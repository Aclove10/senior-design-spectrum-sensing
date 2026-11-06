# Transmitter

Existing files moved here without content changes:

- [primary_tx.grc](primary_tx.grc): editable GNU Radio Companion flowgraph.
- [primary_tx.py](primary_tx.py): generated Python, GNU Radio 3.10.12.0.

The flowgraph connects a complex cosine source through a 0.1 multiplier to a Soapy PlutoSDR sink.

| Setting | Current value |
| --- | --- |
| SDR center frequency | 915 MHz |
| Complex tone offset | +400 kHz |
| Sample rate and configured bandwidth | 2 MS/s and 2 MHz |
| Source amplitude / multiplier | 1 / 0.1 |
| Sink gain setting | 0 |
| Device argument | uri = usb:0.4.5 |

The configured tone is nominally 915.4 MHz; this is a configuration interpretation, not a measured RF result. Gain and amplitude settings are not calibrated output power.

Requires Python 3, GNU Radio with Qt GUI and Soapy support, PyQt5, a PlutoSDR-compatible Soapy driver and device connectivity. Inspect the local URI in Companion before use and regenerate Python if changing it. There is no device-selection CLI in the existing script.

After reviewing the configuration and preparing an approved controlled RF setup, `python3 transmitter/primary_tx.py` from the repository root executes the transmitter. It requires a graphical environment and starts transmission immediately. Use a controlled setup with suitable attenuation and follow the lab's RF operating procedure.

Hardware execution was not performed as part of repository organization.
