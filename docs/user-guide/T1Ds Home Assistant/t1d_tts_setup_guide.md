---
meta:
  - property: og:image
    content: "https://github.com/user-attachments/assets/e6c37552-5970-4f8e-a275-d4181575073f"
---
<!-- this is  on github server!
docs made by D.Galloway 2019- 2026-->


<div align="center">
  <img width="300" height="Auto" border="0" src="https://github.com/user-attachments/assets/f778a2b5-6262-4275-80b9-ef0f16f21e35" title="xdrip+ original logo"/>&emsp;&emsp;
  <img width="95" height="Auto" border="0" src="https://github.com/user-attachments/assets/a029ff04-61a8-4eb0-ba00-0acd214b7c04" title="Dexcom G6 mmol/L DXCM1"/>&emsp;&emsp;
  <img width="95" height="Auto" border="0" src="https://github.com/user-attachments/assets/7607c150-ee98-4f9b-97ff-abb894de6ba0" title="Dexcom Follow mmol/L DXCM1"/>

  <h1 style="text-align: center;"><strong>Dex Share Followers Setup Guide</strong></h1>


<h2 style="text-align: center;"><strong>Setting Up Dexcom Share (Required for Home Assistant)</strong></h2>
</div>


``` { .yaml .copy }
# alias: S24 Announce T1D Glucose Trend From App Dexcom
sequence:
  - delay: "00:00:01"
  - data:
      message: TTS
      data:
        tts_text: >-
          {% set bg = states('sensor.dexcom_g6_clean') | float(0) %}  {% set
          raw_trend = states('sensor.dave247_glucose_trend') %}  {% set
          trend_map = {
            'Flat': 'steady',
            'SingleUp': 'rising',
            'DoubleUp': 'rising quickly',
            'SingleDown': 'falling',
            'DoubleDown': 'falling quickly',
            'FortyFiveUp': 'rising slightly',
            'FortyFiveDown': 'falling slightly'
          } %}  {% set trend = trend_map.get(raw_trend, raw_trend) %}  Blood {{
          bg }} millimoles, and it is {{ trend }}.
        channel: alarm_stream_max
        ttl: 0
        priority: high
    action: notify.mobile_app_sm_s928b
mode: single
icon: mdi:waveform
description: ""
```








```yaml title="S24 Announce T1D Glucose Trend From App Dexcom999999"
alias: S24 Announce T1D Glucose Trend From App Dexcom
sequence:
  - delay: "00:00:01"
  - data:
      message: TTS
      data:
        tts_text: >-
          {% set bg = states('sensor.dexcom_g6_clean') | float(0) %}  {% set
          raw_trend = states('sensor.dave247_glucose_trend') %}  {% set
          trend_map = {
            'Flat': 'steady',
            'SingleUp': 'rising',
            'DoubleUp': 'rising quickly',
            'SingleDown': 'falling',
            'DoubleDown': 'falling quickly',
            'FortyFiveUp': 'rising slightly',
            'FortyFiveDown': 'falling slightly'
          } %}  {% set trend = trend_map.get(raw_trend, raw_trend) %}  Blood {{
          bg }} millimoles, and it is {{ trend }}.
        channel: alarm_stream_max
        ttl: 0
        priority: high
    action: notify.mobile_app_sm_s928b
mode: single
icon: mdi:waveform
description: ""
```
