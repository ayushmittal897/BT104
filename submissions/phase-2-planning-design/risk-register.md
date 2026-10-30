# Risk Register

| Risk | Control |
| --- | --- |
| Dataset leakage | record data split and validation limits |
| Model version mismatch | pin compatible local dependencies |
| Rule false positives | show rule provenance and tune transparently |
| Packet-capture privacy | metadata only; memory only; no PCAP commit |
| API exposure | bind to localhost and restrict CORS |
| Data or secrets pushed to Git | use repository ignore rules |