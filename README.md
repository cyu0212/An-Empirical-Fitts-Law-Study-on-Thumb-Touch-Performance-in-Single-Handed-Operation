# An Empirical Fitts' Law Study on Thumb Touch Performance in Single-Handed Operation
**[Click here to open the Fitts' Law simulator webpage](https://cyu0212.github.io/An-Empirical-Fitts-Law-Study-on-Thumb-Touch-Performance-in-Single-Handed-Operation/)**
## Scenario & Concept

### User & Context
This experiment investigates the motor control performance of commuters operating a smartphone (using an iPhone 13 as the test device) with only a single thumb on crowded public transit. In this context, with one hand occupied (e.g., holding a handrail), the user must rely entirely on one thumb for all screen interactions.

### Real-world HCI Problem
As smartphone screens grow larger (6+ inches), the thumb's comfortable reach—the "Thumb Zone"—is severely limited. Reaching UI elements at the top or edges (e.g., back buttons or close icons) forces excessive thumb stretching or a shift in grip, resulting in two major HCI pain points:
* **Decreased Efficiency & Accuracy:** Muscle strain increases the Movement Time (MT) required to hit targets, while a moving vehicle leads to a higher error rate.
* **Risk of Device Drop:** Shifting the grip reduces phone stability, significantly increasing the risk of dropping the device.

## Experiment Design
* **Physical Touch Test:** Developed a web-based Fitts' Law app tested physically via single-handed interactions on an iPhone 13, replacing traditional mouse clicks to reflect real-world mobile use.
* **Thumb Simulation:** Features a red "OK" button moving along the vertical axis, dynamically simulating the real-world extension and flexion of a user's thumb on a large screen.
* **Dynamic Difficulty:** Systematically varies Target Distance (A) and Target Width (W) to generate varying Indices of Difficulty (ID), allowing precise measurement of thumb Movement Time across different ID levels.
<img width="1891" height="866" alt="image" src="https://github.com/user-attachments/assets/40c6c096-3ffa-416e-a4b2-37408179ad4e" />
<img width="1891" height="863" alt="image" src="https://github.com/user-attachments/assets/0e33f10c-9064-46f2-a598-297a0bece2b5" />
<img width="1896" height="865" alt="image" src="https://github.com/user-attachments/assets/13c16545-1328-4b9a-97e6-dea941f0c565" />

## Experiment Video Link
* **Screen recording:** [https://drive.google.com/file/d/1T7mOY-MxLFpjO7fnIWbvwXaGQVzi3oeR/view?usp=sharing](https://drive.google.com/file/d/1T7mOY-MxLFpjO7fnIWbvwXaGQVzi3oeR/view?usp=sharing)
* **Operation video:** [https://drive.google.com/file/d/1vZjiTcE9ahewerFhKawIKs_F8eorzReN/view?usp=sharing](https://drive.google.com/file/d/1vZjiTcE9ahewerFhKawIKs_F8eorzReN/view?usp=sharing)



https://github.com/user-attachments/assets/e68378b5-cf20-4e28-b172-93193c9f710d


## Fitts' Law Formula
MT = 384.44 + 44.64 * log2(A/W + 1)
* **a:** 384.44
* **b:** 44.64
* **R²:** 0.281

## Parameter Analysis
* **Intercept a (384.44 ms):** Represents "non-movement time". This baseline duration covers visual perception, decision-making, and initial muscle preparation. In a real-world, multitasking commuting environment, this higher value accurately reflects the initial reaction cost of initiating a single-handed operation.
* **Slope b (44.64 ms/bit):** Indicates that for every 1-bit increase in the Index of Difficulty (ID), an additional ~45 ms of movement time is required. When targets are further or smaller, it tests the thumb's fine motor control under extreme extension.
* **R² (0.281):** While traditional desktop mouse experiments usually yield an R² > 0.9, this experiment resulted in only 0.281. This surprisingly low value is a highly valuable empirical finding, proving that "single-handed operation of large-screen phones" is a highly unstable interaction process subject to multiple interfering variables. The main reasons for the high data variance (huge time differences under the same ID) include:
  * **Non-linear Workspace:** The thumb moves in a fan-shaped trajectory rather than a perfect 2D plane, making ergonomic difficulty vary drastically when reaching for different corners.
  * **Dynamic Grip Compensation:** To reach the extreme edges of the screen, users must slightly adjust their palm's grip center, introducing unpredictable time delays.

## Implications for HCI Design
* **Establish a Thumb Golden Zone:** Because the top and diagonal areas of large-screen phones are difficult to reach (excessive Distance A leads to high latency and low stability), important core function buttons (e.g., confirm payment, send messages, navigation bars) should be concentrated within the natural thumb movement arc in the lower-middle section of the screen.
* **Dynamic Adjustment for Edge Targets:** According to Fitts' Law, if UI elements (such as the 'X' to close a window or the back button) must inevitably be placed at hard-to-reach screen edges, designers must significantly enlarge their "invisible clickable area" (increase Width W). By artificially lowering the Index of Difficulty (ID), designers can effectively compensate for the operational costs and misclick risks caused by distance.
