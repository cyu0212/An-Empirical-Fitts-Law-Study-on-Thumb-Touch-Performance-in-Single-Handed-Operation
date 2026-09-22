# An Empirical Fitts' Law Study on Thumb Touch Performance in Single-Handed Operation[cite: 3]

## Scenario & Concept[cite: 3]

### User & Context[cite: 3]
This experiment investigates the motor control performance of commuters operating a smartphone (using an iPhone 13 as the test device) with only a single thumb on crowded public transit[cite: 3]. In this context, with one hand occupied (e.g., holding a handrail), the user must rely entirely on one thumb for all screen interactions[cite: 3].

### Real-world HCI Problem[cite: 3]
As smartphone screens grow larger (6+ inches), the thumb's comfortable reach—the "Thumb Zone"—is severely limited[cite: 3]. Reaching UI elements at the top or edges (e.g., back buttons or close icons) forces excessive thumb stretching or a shift in grip, resulting in two major HCI pain points[cite: 3]:
* **Decreased Efficiency & Accuracy:** Muscle strain increases the Movement Time (MT) required to hit targets, while a moving vehicle leads to a higher error rate[cite: 3].
* **Risk of Device Drop:** Shifting the grip reduces phone stability, significantly increasing the risk of dropping the device[cite: 3].

## Experiment Design[cite: 3]
* **Physical Touch Test:** Developed a web-based Fitts' Law app tested physically via single-handed interactions on an iPhone 13, replacing traditional mouse clicks to reflect real-world mobile use[cite: 3].
* **Thumb Simulation:** Features a red "OK" button moving along the vertical axis, dynamically simulating the real-world extension and flexion of a user's thumb on a large screen[cite: 3].
* **Dynamic Difficulty:** Systematically varies Target Distance (A) and Target Width (W) to generate varying Indices of Difficulty (ID), allowing precise measurement of thumb Movement Time across different ID levels[cite: 3].

## Experiment Video Link[cite: 3]
* **Screen recording:** [https://drive.google.com/file/d/1T7mOY-MxLFpjO7fnIWbvwXaGQVzi3oeR/view?usp=sharing](https://drive.google.com/file/d/1T7mOY-MxLFpjO7fnIWbvwXaGQVzi3oeR/view?usp=sharing)[cite: 3]
* **Operation video:** [https://drive.google.com/file/d/1vZjiTcE9ahewerFhKawIKs_F8eorzReN/view?usp=sharing](https://drive.google.com/file/d/1vZjiTcE9ahewerFhKawIKs_F8eorzReN/view?usp=sharing)[cite: 3]

## Fitts' Law Formula[cite: 3]
MT = 384.44 + 44.64 * log2(A/W + 1)[cite: 3]
* **a:** 384.44[cite: 3]
* **b:** 44.64[cite: 3]
* **R²:** 0.281[cite: 3]

## Parameter Analysis[cite: 3]
* **Intercept a (384.44 ms):** Represents "non-movement time"[cite: 3]. This baseline duration covers visual perception, decision-making, and initial muscle preparation[cite: 3]. In a real-world, multitasking commuting environment, this higher value accurately reflects the initial reaction cost of initiating a single-handed operation[cite: 3].
* **Slope b (44.64 ms/bit):** Indicates that for every 1-bit increase in the Index of Difficulty (ID), an additional ~45 ms of movement time is required[cite: 3]. When targets are further or smaller, it tests the thumb's fine motor control under extreme extension[cite: 3].
* **R² (0.281):** While traditional desktop mouse experiments usually yield an R² > 0.9, this experiment resulted in only 0.281[cite: 3]. This surprisingly low value is a highly valuable empirical finding, proving that "single-handed operation of large-screen phones" is a highly unstable interaction process subject to multiple interfering variables[cite: 3]. The main reasons for the high data variance (huge time differences under the same ID) include[cite: 3]:
  * **Non-linear Workspace:** The thumb moves in a fan-shaped trajectory rather than a perfect 2D plane, making ergonomic difficulty vary drastically when reaching for different corners[cite: 3].
  * **Dynamic Grip Compensation:** To reach the extreme edges of the screen, users must slightly adjust their palm's grip center, introducing unpredictable time delays[cite: 3].

## Implications for HCI Design[cite: 3]
* **Establish a Thumb Golden Zone:** Because the top and diagonal areas of large-screen phones are difficult to reach (excessive Distance A leads to high latency and low stability), important core function buttons (e.g., confirm payment, send messages, navigation bars) should be concentrated within the natural thumb movement arc in the lower-middle section of the screen[cite: 3].
* **Dynamic Adjustment for Edge Targets:** According to Fitts' Law, if UI elements (such as the 'X' to close a window or the back button) must inevitably be placed at hard-to-reach screen edges, designers must significantly enlarge their "invisible clickable area" (increase Width W)[cite: 3]. By artificially lowering the Index of Difficulty (ID), designers can effectively compensate for the operational costs and misclick risks caused by distance[cite: 3].
