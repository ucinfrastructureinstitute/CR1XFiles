# CR1XFiles
1) trail.CR1X
Purpose: Basic template trail monitoring program.
Features:
- Reads sensor inputs connected to the datalogger.
- Applies scan intervals and logging conditions.
- Stores data in a table for later retrieval.
Notes: This program is intended as the baseline configuration for trail data collection.

2) trailBattVolt.CR1X
Purpose: Battery voltage monitoring program.
Features:
- Measures the CR1000X system battery voltage at regular intervals.
- Logs voltage readings to track power stability.
- Can be used to diagnose low-power events or ensure sufficient power supply in remote deployments.
Notes: This program can be run standalone or alongside sensor-logging programs for power diagnostics.

3) trail[usingTWOvwire305].CR1X
Purpose: Monitoring using dual VWIRE305 modules.
Features:
- Configured to interface with two Campbell VWIRE305 vibrating-wire interfaces.
- Captures strain, frequency, or other VWIRE sensor data.
- Logs synchronized readings from both modules for comparison or redundancy.
Notes: Useful for setups requiring multiple vibrating-wire measurements.

Usage Instructions
- Upload the desired .CR1X file to the CR1000X datalogger using LoggerNet.
- Ensure that connected sensors and wiring match the program setup (e.g., VWIRE305 channels, power supply).
- Confirm table definitions and adjust scan intervals as needed for your deployment.
