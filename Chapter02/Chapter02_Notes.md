---
title: "The Art Of Electronics 3rd Edition - Notes on Chapter 02"
date: 2023-11-08
geometry: margin=2cm
output: pdf_document
---

# Exercise 2.2

Charging from -4.4 V to +5 V :

$$
V_{B_{Q_2}} = (5 - (-4.4)) \cdot e^{-t/\tau} + (-4.4)
= 9.4 \cdot e^{-t/\tau} - 4.4
$$

The pulse ends when Q2 turns on again, so when $V_{B_{Q_2}} = 0.6~V$:

$$
0.6 = 9.4 \cdot e^{-t/\tau} - 4.4
$$
$$
t = -\tau \cdot ln(1-\frac{5}{9.4}) = -0.76 \cdot \tau
$$