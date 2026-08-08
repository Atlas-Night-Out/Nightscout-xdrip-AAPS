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
