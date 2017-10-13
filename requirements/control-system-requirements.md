# Control System Requirements

#### Introduction

For our project we aim to build a plane capable of autonomous flight, including take-off and landing, automatic payload delivery and endurance. To make this possible, the control system requires a powerful CPU capable of filtering sensor data effectively, various sensors and means of communicating wirelessly, while also ensuring safe operation. This document aims to list all control requirements and state their importance.

#### Functional Requirements {#control-requirements}

| ID | Requirement | Importance \(MoSCoW\) |
| :---: | :--- | :---: |
| CSR:F001 | Control system should enable, on command, autonomous takeoff of the aircraft within 30m of starting location | Should |
| CSR:F002 | Control system should enable, on command, autonomous landing of the aircraft within 30m area, including touchdown and rollout | Should |
| CSR:F003 | Control system should enable autonomous navigation of predefined GPS waypoints, with an accuracy of within 2 metres | Should |
| CSR:F004 | Control system must provide real-time telemetry during a mission to allow observing flight and sensor data and modification of mission in-flight | Must |
| CSR:F005 | Control system must be modular to allow a quick replacementif a component fails | Must |
| CSR:F006 | Control system must include a 32-bit CPU Flight Controller to allow use of Kalman filters | Must |
| CSR:F007 | Control system must have an inertial measurement unit, including a 3-axis accelerometer and 3-axis gyroscope to estimate linear and angular speeds and positions | Must |
| CSR:F008 | Control system must include a barometer to estimate altitude | Must |
| CSR:F009 | Control system must include GPS to get more accurate estimates on position, plus additional data improves overall estimates thanks to Kalman filter | Must |
| CSR:F010 | Control system must accurate \(&lt; 1m\) altitude measuring capability, for example LIDAR,as reliable altitude data is needed to control landing process and time of flaring | Must |
| CSR:F011 | Control system must include an airspeed sensor to control landing approach autonomously | Must |
| CSR:F012 | Control system could provide on-board display unit to simplify pre-arm checks | Could |
| CSR:F013 | Control system must use radio equipment compliant with EU standard EN 300 328, as required by the competition rules | Must |
| CSR:F014 | Control system must use rado equipment which is ‘Spread Spectrum’ compliant, as required by the competition rules | Must |
| CSR:F015 | Control system could implement a location finder system, activated upon crash landing, to aid locating the airframe | Could |

#### Safety Requirements

| ID | Requirement | Importance \(MoSCoW\) |
| :--- | :--- | :--- |
| CSR:S001 | Control system must be incorporate a Flight Termination System, as mandated by the competition rules, both automatically activated on loss of communication with aircraft and manually selectable by the operator | Must |
| CSR:S002 | Control system must prosecute Flight Termination System commands within 10 seconds of activation or uplink loss | Must |
| CSR:S003 | Control system must be return received signal strength indication to the ground station, to ensure uplink integrity | Must |
| CSR:S004 | Control system must include an additional transmitter, in buddy box configuration, for use by the Flight Safety Officer at competition | Must |
| CSR:S005 | Control system must use radio equipment with a range of at least 1km | Must |



