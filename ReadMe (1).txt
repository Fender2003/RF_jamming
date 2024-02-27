# RF Jamming Dataset for Vehicular Wireless Networks

## Overview

This dataset contains measurements and ground truth labels used for research in the paper "RF Jamming Classification Using Relative Speed Estimation in Vehicular Wireless Networks." It is designed to support the development and evaluation of detection algorithms for RF jamming attacks in Vehicular Ad-hoc Networks (VANETs).

## Dataset Columns

The dataset consists of the following columns:

- `Time`: The timestamp of the measurement.
- `SNR` (Signal-to-Noise Ratio): A measure of the signal quality.
- `Speed`: The speed of the vehicles involved in the communication.
- `RSSI` (Received Signal Strength Indicator): A measurement of signal strength.
- `PDR` (Packet Delivery Ratio): The ratio of successfully delivered packets.
- `Relative_Speed`: The variations in estimated relative speed between the jammer and the receiver.
- `Scenario`: A numerical code representing the scenario: 1 (No Attack), 2 (Reactive Attack), 3 (Constant Attack).

## Scenarios in the Datasets

The dataset includes three distinct scenarios, denoted as Scenario 1, Scenario 2, and Scenario 3. Each scenario represents a potential jamming attack case that may occur in a real-world environment.

- Scenario 1 (No Attack):  The situation is examined in which there is an absence of a jammer, but there exists a source of unintentional interference that impacts the communication between the receiver and the transmitter. The objective of creating and simulating this specific scenario is to assess the capability of the VRS feature in distinguishing interference from intentional jamming. Such capability is deemed critical and necessary, particularly in an urban environment where interference is a significant factor contributing to wireless communication disruption. The receiver's vehicle travels through an area with significant interference, resulting in an immediate disruption of its communication with the transmitter (another vehicle or an RSU).
- Scenario 2 (Reactive Jammer Attack): The scenario involves the presence of a jammer that initiates following the target from an initial position (specified as one of the simulation parameters) while simultaneously transmitting jamming signals. As the jammer approaches the target, the jamming signals become more powerful, resulting in a more intense disruption of communication between the receiver and the transmitter. When the jammer reaches the target, in order to remain undetected for as long as possible, it retreats to a safe distance from which it periodically transmits jamming signals. The specific retreat location and the rate of jamming signal transmission are randomly determined for each simulation, with the safety distance ranging from 5 to 10 meters and the frequency of jamming signal transmission varying between 5 and 15 times per unit period.
- Scenario 3 (Constant Jammer Attack): The scenario examines a situation in which a constant jammer persistently transmits jamming signals while continuously following the target. When the jammer reaches its target, it begins transmitting at maximum power without the intention of remaining undetected.


## Datasets

- Dataset_1: 25m/s is used as the maximum estimated relative speed, which is the absolute value of the jammer speed minus the receiver speed.
- Dataset_2: 15m/s is used as the maximum estimated relative velocity.


## Usage

Researchers and practitioners in the field of wireless communication security can utilize this dataset to:

- Develop and evaluate RF jamming detection algorithms.
- Study the impact of different scenarios on detection accuracy.
- Investigate the role of features such as relative speed (VRS) in jamming detection.

## Citation

If you use this dataset in your research or work, please consider citing the original paper:

**D. Kosmanos, D. Karagiannis, A. Argyriou, S. Lalis, and L. Maglaras, "RF Jamming Classification Using Relative Speed Estimation in Vehicular Wireless Networks." Security and Communication Networks, Hindawi, 2021, DOI: 10.1155/2021/9959310.

## Acknowledgments

We would like to acknowledge the original paper's authors for creating and sharing this dataset.


