


<!-- docs made by D.Galloway 2019 - 2026 -->

# Lovelace T1D Diabetes Card for Home Assistant

The **Lovelace T1D Diabetes Card** brings your full AndroidAPS, Nightscout, and CGM data right into your Home Assistant dashboards. It is designed for clear glanceability, sensor tracking, and direct voice integration with Alexa devices across your home.

<p align="center">
  <img src="../../../img/T1Ds Home Assistant/T1DDiabetesCard.png" width="220" title="Lovelace T1D Diabetes Card Preview" alt="Lovelace T1D Diabetes Card Preview" />
</p>

> ⚠️ **Development Status:** Work in progress! Final fixes and updates are being actively worked on with a target to have it fully polished and working correctly this week (aiming for Friday).

---

## 🌟 Key Features & Interface Breakdown

### 📊 Real-Time CGM & Metrics
* **Glucose Readout & Trend:** Displays current mmol/L (e.g., `4.3 mmol/L Steady ➔`) with an integrated ring indicator.
* **Treatment Stats:** Live tracking for **IOB** (Insulin on Board), **COB** (Carbs on Board), and **REQ** (Basal Request).
* **Estimated A1C:** Calculated live estimation based on recent glucose logs.
* **Glucose History Graph:** Compact trend line and detailed 24-hour range chart showing high/low thresholds (`10.5` / `4.0`).

### ⏳ Sensor Expiry & Countdown
* **Sensor Days Tracker:** Shows the exact remaining lifespan of your active sensor (`e.g., 2 days, 2 hours, and 46 minutes`).
* Helps you plan exactly when your sensor end date/replacement is due so you never get caught off guard.

### 🗣️ Alexa Voice Readouts (AAPS via TTS)
* Built-in direct trigger buttons (**T1D Livingroom Readout** & **T1D Bedroom Readout**).
* Tapping these triggers Home Assistant scripts to send voice announcements over your Echo devices (Echo Show 10, etc.), reading out current AAPS readings, trend directions, and warnings loud and clear without opening the app.

---

## 🚀 Installation & Setup

### Option 1: Installation via HACS (Recommended)

1. Open **HACS** in Home Assistant.
2. Go to **Frontend** ➔ Click the **3 dots** (top right) ➔ Select **Custom Repositories**.
3. Add repository URL:
   `https://github.com/Atlas-Night-Out/lovelace-t1d-diabetes-card`
4. Category: **Lovelace**.
5. Click **Add**, find the card in HACS, and click **Download**.

---

### Option 2: Manual Installation

1. Download `lovelace-t1d-diabetes-card.js` from the [GitHub Repository](https://github.com/Atlas-Night-Out/lovelace-t1d-diabetes-card).
2. Save the file in your Home Assistant `/config/www/` folder.
3. Add the resource under **Settings** ➔ **Dashboards** ➔ **Resources**:
   * **URL:** `/local/lovelace-t1d-diabetes-card.js`
   * **Resource Type:** `JavaScript Module`

---

## 🔗 Repository & Support

* **Source Code:** [GitHub - Atlas-Night-Out/lovelace-t1d-diabetes-card](https://github.com/Atlas-Night-Out/lovelace-t1d-diabetes-card)
* **Issues & Bug Tracker:** [Report Issues on GitHub](https://github.com/Atlas-Night-Out/lovelace-t1d-diabetes-card/issues)


<br>

<br>

[&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;]()
[Please Subscribe to our UTUBE Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button }

<br>
<a href="https://maundyrelief.org.uk/" target="_blank">
  <center><img width="300" height="auto" border="0" align=""  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/></center></a>
<br>

<br>
<a href="https://www.diabetes.org.uk/" target="_blank">
<img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/> </a>Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank"> :man_biking_tone1: UK Wide Cycle Ride - Diabetes.uk :woman_biking_tone5:</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22 :man_swimming_tone5:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank">:man_walking_tone5: Diabetes UK Month of Miles Challenge :woman_running:</a> for all of your Diabetes Needs!