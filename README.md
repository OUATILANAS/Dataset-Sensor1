# Cloud-Local LoRaWAN Greenhouse Dataset

This repository contains the sensor-reading dataset used in the revised manuscript:

**A Local-First LoRaWAN Observability Layer for XR-Ready Greenhouse Digital Twin Supervision with Nexelec RISE Sensors**

The dataset supports the evaluation of a local-first LoRaWAN observability platform for greenhouse climate supervision. It includes decoded environmental readings and communication metadata collected from Nexelec RISE sensors through a MultiTech Conduit LoRaWAN gateway.

## Repository content

| File | Description |
|---|---|
| `recovered-data-updated-5434-readings.xlsx` | Main recovered dataset containing 5,434 decoded sensor-reading records. |
| `README.md` | Dataset description, usage notes, and citation information. |

## Dataset overview

The dataset contains **5,434 decoded readings** from a greenhouse LoRaWAN monitoring prototype. It is intended to support reproducible analysis of local-first IoT observability, packet traceability, and environmental monitoring.

Main characteristics:

- **Total records:** 5,434 decoded sensor readings
- **Sensor type:** Nexelec RISE environmental sensors
- **Gateway:** MultiTech Conduit LoRaWAN gateway
- **Measured variables:** CO₂, temperature, relative humidity, and derived VPD when available
- **Communication metadata:** device identity, gateway context, RSSI, SNR, frequency, f-port, timestamps, and sequence/count information when available
- **Purpose:** evaluation of data ingestion, local storage, dashboard supervision, packet traceability, and local-first observability

## Research context

The dataset was used to strengthen the quantitative evaluation of a LoRaWAN greenhouse supervision architecture. The revised work compares cloud-first, hybrid, and local-first monitoring approaches, with a focus on preserving both environmental readings and communication evidence.

The dataset is not presented as proof of crop-yield improvement, water savings, disease-risk reduction, autonomous control, or industrial-grade reliability. It is used as prototype evidence for IoT observability and XR-ready greenhouse digital-twin data trust.

## Typical fields

Depending on the exported sheet structure, the dataset may include fields such as:

- Reading identifier
- Sensor/device identifier or DevEUI
- Timestamp / received time / created time
- CO₂ value in ppm
- Temperature in °C
- Relative humidity in %
- Vapour pressure deficit (VPD) in kPa
- RSSI in dBm
- SNR in dB
- LoRaWAN frequency in MHz
- Gateway identifier or gateway count
- f-port
- Source or status fields

## Suggested use

This dataset can be used for:

- Greenhouse environmental data analysis
- LoRaWAN packet-delivery and sequence-gap analysis
- Radio-metadata analysis using RSSI, SNR, and frequency
- Local-first IoT observability studies
- Preparation of XR-ready or digital-twin greenhouse supervision backends
- Reproducible comparison between cloud and local monitoring approaches

## Data availability statement

The dataset is publicly available in this GitHub repository:

```text
https://github.com/quaboam/Cloud-Local-LoRaWAN-Greenhouse-Dataset
```

Suggested statement for the manuscript:

> The dataset used in this study is available through the project GitHub repository: https://github.com/quaboam/Cloud-Local-LoRaWAN-Greenhouse-Dataset.

## Funding acknowledgement

This work was financially supported by the **“Jeunes Chercheurs” program of Cadi Ayyad University**, through which key research equipment used in this study was acquired. Additional material support was provided through the **Living Lab ResilientCity** international structuring partnership involving Gustave Eiffel University and Cadi Ayyad University.

## Citation

If you use this dataset, please cite the associated manuscript:

```text
Ouatil, A., Abouzahir, S., El Kabtane, H., and Tajer, A.
A Local-First LoRaWAN Observability Layer for XR-Ready Greenhouse Digital Twin Supervision with Nexelec RISE Sensors.
Submission 100, ICVR 2026.
```

## Contact

For questions about the dataset or manuscript, please contact:

**Anas Ouatil**  
LISA Laboratory, ENSA, Cadi Ayyad University  
Marrakesh, Morocco  
Email: a.ouatil.ced@uca.ac.ma

## License

Add your preferred license here before publication. Recommended options include:

- `CC BY 4.0` for open academic reuse with attribution
- `CC BY-NC 4.0` if you want to restrict commercial use
- `MIT License` only if the repository also contains reusable code

