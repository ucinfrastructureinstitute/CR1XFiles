****1. trail.CR1X**

**Purpose:****
Basic template trail monitoring program.

**Features:**
Reads sensor inputs connected to the datalogger.
Applies scan intervals and logging conditions.
Stores data in a table for later retrieval.

**Notes:**
This program is intended as the baseline configuration for trail data collection.

**2. trail[microSDcard].CR1X**

**Purpose:**
Trail monitoring program configured to log data directly to a microSD card.

**Features:**
Same sensing and scan logic as the base trail program.
Enables storage and retrieval via external microSD media.
Adds periodic data flushing for power stability.

**Notes:**
Useful when remote deployment requires offline data storage or limited LoggerNet connectivity.

**3. trail[usingTWOvwire305] **

**Purpose:**
Trail monitoring program supporting dual VWIRE 305 analyzers.
**Features:**
Reads from two vibrating-wire sensor channels simultaneously.
Synchronizes sampling between analyzers.
Logs temperature and strain data for multiple sensors.

**Notes:**
Designed for setups with multiple VW sensors per location or when redundancy is needed.

**4. trailBattVolt.CR1X**

**Purpose:**
Trail monitoring with integrated battery voltage measurement.

**Features:**
Adds periodic checks of system voltage.
Logs power supply trends alongside environmental data.
Alerts or flags low-voltage conditions.

**Notes:**
Recommended for long-term deployments where battery health monitoring is critical.

**5. 30minOFF9secON[workinggood].CR1X**

**Purpose:**
Optimized low-power trail monitoring program with duty-cycling.

**Features:**
Powers system ON for 9 seconds every 30 minutes for data acquisition.
Collects and logs sensor data during each ON cycle.
Greatly reduces overall energy consumption.

**Notes:**
Verified working configuration; best suited for remote solar or battery-powered stations.

**6. sisterbar.CR1X**

**Purpose:**
Sister bar monitoring program for structural or tension measurements.

**Features:**
Acquires strain and temperature readings from vibrating-wire gauges on sister bars.
Logs data at predefined scan intervals.
Provides baseline tension or stress monitoring.

**Notes:**
Serves as a companion configuration to trail.CR1X for additional structural measurement points.

**Usage Instructions**
- Upload the desired .CR1X file to the CR1000X datalogger using LoggerNet.
- Ensure that connected sensors and wiring match the program setup (e.g., VWIRE305 channels, power supply).
- Confirm table definitions and adjust scan intervals as needed for your deployment.
