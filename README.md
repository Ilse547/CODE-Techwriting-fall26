# ForestGuard 🌲🔥

**Rapid wildfire detection and emergency alert system for communities.**

---

## Description

ForestGuard is a community-driven platform designed to empower individuals to report suspected wildfires instantly to local authorities. By streamlining the communication between eyewitnesses and emergency services, ForestGuard aims to reduce response times during critical early stages of a fire. The application allows users to submit geolocated reports with photos, descriptions, and severity estimates, which are then automatically routed to the nearest fire department dispatch center.

## Quick Start

To get started with ForestGuard immediately:

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/your-org/forestguard.git
    cd forestguard
    ```

2.  **Install dependencies**:
    ```bash
    npm install
    # or
    pip install -r requirements.txt
    ```

3.  **Run the application**:
    ```bash
    npm start
    # or
    python app.py
    ```

4.  **Access the dashboard**:
    Open your browser and navigate to `http://localhost:3000`.

## Usage

### Reporting a Fire
1.  Log in to your account (or use the guest emergency mode).
2.  Click the **"Report Wildfire"** button.
3.  Allow location permissions or manually adjust the map pin.
4.  Upload photos or videos of the smoke/fire if safe to do so.
5.  Select the estimated size and intensity from the dropdown menu.
6.  Submit the report. An automated confirmation will be sent, and the alert is forwarded to authorities.

### Viewing Active Alerts
Authorized personnel and community moderators can view a real-time heat map of active reports, filter by severity, and track the status of dispatched units.

## Configuration

Create a `.env` file in the root directory to configure environment variables:

```env
# Database Connection
DATABASE_URL=postgresql://user:password@localhost:5432/forestguard

# API Keys
EMERGENCY_API_KEY=your_emergency_service_api_key
MAPBOX_TOKEN=your_mapbox_access_token

# Server Settings
PORT=3000
NODE_ENV=development

# Notification Settings
SMTP_HOST=smtp.example.com
SMTP_PORT=587
ALERT_EMAIL=noreply@forestguard.org
