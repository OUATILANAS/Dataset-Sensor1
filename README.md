# Cloud-Local LoRaWAN Greenhouse Dataset

This repository contains the cleaned merged sensor-reading dataset used in the revised manuscript:

**A Local-First LoRaWAN Observability Layer for XR-Ready Greenhouse Digital Twin Supervision with Nexelec RISE Sensors**

The dataset supports the evaluation of a local-first LoRaWAN observability platform for greenhouse climate supervision. It includes decoded environmental readings and LoRaWAN communication metadata collected from Nexelec RISE sensors through a MultiTech Conduit LoRaWAN gateway.

## Repository content

| File | Description |
|---|---|
| `recovered_data.xlsx` | Cleaned merged sensor-reading dataset containing 6,222 records from five Nexelec RISE devices. |
| `README.md` | Dataset description, usage notes, data-quality notes, and citation information. |

## Dataset overview

The dataset contains **6,222 decoded sensor-reading records** from a greenhouse LoRaWAN monitoring prototype. It is intended to support reproducible analysis of local-first IoT observability, environmental monitoring, packet traceability, and XR-ready greenhouse digital-twin data trust.

Main characteristics:

- **Total sensor-reading records:** 6,222
- **Unique reading identifiers:** 5,788
- **Reading ID range:** 1 to 5,788
- **Missing ID gaps:** 0
- **Duplicated identifiers:** 434 duplicated IDs; IDs 1–434 appear twice after merging
- **Number of devices:** 5 DevEUIs
- **Records per device:** 1,219 to 1,290 records per device
- **Date span:** 2026-05-19 18:55:41 to 2026-07-07 23:54:46 UTC
- **Gateway ID:** 00800000D00099D6
- **LoRaWAN f-port:** 56
- **Measured variables:** CO₂, temperature, relative humidity, and derived VPD
- **Communication metadata:** device identity, gateway context, RSSI, SNR, frequency, timestamps, f-port, and sequence/count information when available
- **Purpose:** evaluation of data ingestion, local storage, dashboard supervision, communication traceability, and local-first observability

## Data-quality note

This cleaned merged dataset contains only the **sensor-reading** data used for the revised quantitative analysis.

The dataset contains **434 duplicated reading identifiers** because IDs 1–434 appear twice after merging. These duplicated identifiers are kept and reported as a data-quality boundary rather than hidden. They should be considered during reproducible analysis, especially when computing counts based on unique identifiers.

The dataset has **no missing reading-ID gaps** in the ID range 1–5,788.

## Descriptive statistics

| Variable | n | Minimum | Median | Mean | Maximum |
|---|---:|---:|---:|---:|---:|
| CO₂ stored value (ppm) | 6,222 | 0.0 | 483.5 | 492.8 | 943.0 |
| Temperature (°C) | 6,222 | 18.0 | 24.4 | 24.6 | 41.0 |
| Relative humidity (%) | 6,222 | 17.5 | 57.3 | 56.4 | 74.2 |
| VPD (kPa) | 6,222 | 0.55 | 1.30 | 1.46 | 6.41 |
| RSSI (dBm) | 6,222 | -118.0 | -67.0 | -66.2 | -14.0 |
| SNR (dB) | 6,222 | -13.0 | 7.0 | 6.8 | 14.0 |
| Frequency (MHz) | 6,222 | 867.1 | 867.9 | 867.8 | 868.5 |

## Research context

The dataset was used to strengthen the quantitative evaluation of a LoRaWAN greenhouse supervision architecture. The revised work compares cloud-first, hybrid, and local-first monitoring approaches, with a focus on preserving environmental readings and communication evidence for traceable greenhouse supervision.

The dataset is not presented as proof of crop-yield improvement, water savings, disease-risk reduction, autonomous control, or industrial-grade reliability. It is used as prototype evidence for IoT observability, local data trust, and XR-ready greenhouse digital-twin backend preparation.

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
- LoRaWAN sequence-gap and data-quality analysis
- Radio-metadata analysis using RSSI, SNR, and frequency
- Local-first IoT observability studies
- Preparation of XR-ready or digital-twin greenhouse supervision backends
- Reproducible comparison between cloud and local monitoring approaches

## Data availability statement

The dataset is publicly available in this GitHub repository:

```text
https://github.com/OUATILANAS/Dataset-Sensor1
```

Suggested statement for the manuscript:

> The cleaned merged sensor-reading dataset used in this study is available through the project GitHub repository: https://github.com/OUATILANAS/Dataset-Sensor1.

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
