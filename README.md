Waterproof Raspberry Pi Camera Pan-Tilt Mechanism

This project features a fully weather-proof pan and tilt camera bracket controlled by Bowden cables, specifically designed for MIPI cameras like those used with the Raspberry Pi.
Overview

<p align="center">
  <img src="https://cdn.hackaday.io/images/1437081774818601577.JPG" width="600" alt="Pan Tilt Mechanism">
</p>

Traditional pan-tilt systems often have motors attached directly to moving parts, making weather-proofing difficult and expensive. This design moves the electric actuators remotely under a weather-proof canopy or enclosure, reducing both complexity and cost.
Key Features

    Remote Control: Controlled by linear actuators hidden safely away.

    Torsion Springs: Used to act against the cables, as Bowden cables typically only operate in "pull" mode.

    Weather-proof Enclosure: Includes a square IP68 enclosure for the camera.

    Durability: The design is "beefy" enough to survive a knock from a stray 3" tree branch.

Supplies
Hardware

    Bolts: 2x M5 x 70mm, 4x M5 x 40mm CS, 1x M5 x 25mm CS.

    Nuts: 7x M5 nyloc nuts.

    Cables: Bowden cables (1.5mm+sheath×3m) and 4x cable end lugs (OD 5mm x 7mm).

    Springs:

        1x 2mm THK, 7 coils, 90 degrees.

        2x 1.5mm THK, 4 coils, 180 degrees.

    Electronics: 500mm camera ribbon cable and a 20mm cable gland.

    Enclosure: Hammond 1554B2GYCL Watertight PC Enclosure (65×65×40mm).

3D Printed Parts

Most components are 3D printed in SLA resin (standard PLA is also used) for under $60.

    CAD Files: Available on GitHub.

    Note: The swivel connector must be built from stainless steel as plastic versions tend to snap under pressure.

Testing the Mechanism

Initial testing was performed by bolting the assembly to a pallet and using mole grips to simulate linear actuator movement.
Critical Findings:

    Cable Length: 200mm cables were too short and caused internal tension that interfered with movement. At least one meter of cable is recommended for final installation.

    Spring Selection: Trial and error is required. Overpowered springs stress components, while light springs cannot overcome cable friction.

    Pin Reinforcement: The tilt pin is a common failure point. This design uses a 3D-printed pin with a center hole, reinforced by sliding a 2mm spring steel rod inside.

Assembly Instructions
1. Base and Pan Mechanism

    Begin with the base disc. Slide a matching spring steel pin into the center hole of the 3D-printed pin to reinforce the plastic.

    Insert a nyloc nut into the hexagonal captive slot.

    Attach the Bowden cables using the metal lugs (screwed and soldered for security).

    Slot the two main pieces together and secure with a 25mm M5 bolt. Keep it loose enough for the discs to spin without friction.

    Connect the cable to the pin using the stainless steel swivel connector. Attach the heavy-duty spring (2mm THK) so it acts against the pin.

2. Tilt Mechanism

    Use a 70mm bolt and the two 1.5mm springs.

    Place the springs at either end of the bolt and secure with a nyloc nut.

    Ensure the mechanism takes a bit of force to push back; this ensures a steady camera.

3. Camera Enclosure and Weather-proofing

    Mount the Raspberry Pi AI camera inside the Hammond enclosure using a 3D-printed bracket.

    Pro Tip: Position the lens as close to the clear lid as possible to prevent glares and blurry spots.

    Pass the 16mm ribbon cable through the cable gland.

    To ensure a 100% waterproof seal, use a rubber O-ring and fill the inside of the gland with epoxy resin.

Project sponsored by PCBWay. https://www.pcbway.com/
