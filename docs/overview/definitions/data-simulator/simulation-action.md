---
layout: default
title: Data Simulator (Actions)
parent: Data Simulator
grand_parent: Key Concepts
---
# Data Simulation (Actions)
The actions that expect a response from another server can mock the expected response. The mock result feature can be turned on and off by clicking the check box **[C]**. The mock result is switched ON by default to avoid making unwanted calls to the server

The simulated mock data **[A]** is made available throughout the flow **[B]**.   

![Data Simulation Action](/assets/images/data-simulation-action.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> After you have configured the action, switch the mock data OFF **[A]** to receive the real data from the Server.  Cut and paste the data **[B]** back into the action’s mock data **[C]**. That way you are using the mocked data based on the real response.
>
> ![Data Simulation Action](/assets/images/data-simulation-action-flow.png)

> IMPORTANT ** Mock data only exists within the product**
>
> That means it's a good practice to perform a test with the real data once you complete building the solution with the mock data.
