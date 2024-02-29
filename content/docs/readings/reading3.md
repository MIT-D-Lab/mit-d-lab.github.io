---
title: Reading 3 — Introduction to Sensors + Signal Processing
next: reading4
math: true
---

The questi

![](../../../images/gauss.jpg)

statistical model of a sensor? 

![](../../../images/error.png)

Let's say I have a sensor with an accuracy of $a,$ then the reading from the sensor could be:

$$T - a <= T <= T + a$$

Where $T$ is the true value the sensor is trying to measure. But we're continuously measuring the sensor right? Every so often we're going to take a new measurement. And the maximum "error" between any two measurements can be given based on the following.

$$T_1 - a <= T_1 <= T_1 + a$$
$$T_2 - a <= T_2 <= T_2 + a$$

The maximum error is when the sensor reads the highest value it possibly can, and it reads the lowest value it possibly can. And vice versa. 

$$(T_2 - a) - (T_1 + a) <= T_2-T_1 <= (T_2 - a) - (T_1 + a)$$
$$(T_2 - T_1) - 2a <= T_2-T_1 <= (T_2 - T_2) + 2a$$

If you didn't follow this math, that's OK. **But the main idea, is you need your sensors to have an accuracy twice as good as your allowable error range.**


### Now also --> what if the above is *shifted* what if we have a precision window but it's not symmetric?