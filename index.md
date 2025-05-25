# Clay Under Load – A Visual Introduction to Undrained, Consolidation, and Safety Stages

This page presents a simplified numerical model built in [**PLAXIS**](https://www.plaxis.com/) to illustrate how saturated soft clay responds to surface loading through three typical **phases** of geotechnical analysis: **undrained plastic**, **consolidation**, and **safety**.

These phases were simulated using the [PLAXIS Finite Element software](https://www.plaxis.com/), widely used in geotechnical engineering.

<p align="center">
  <img src="assets/plaxis-logo.png" alt="PLAXIS logo" style="width: 150px;">
</p>

---

<h2>🧱 Model Overview</h2>

<div style="display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 20px;">

  <div style="flex: 1; min-width: 300px;">
    <p>
      This 2D plain strain model represents a <strong>6-meter thick saturated clay layer</strong> loaded at the surface in three steps. The clay is <strong>normally consolidated</strong>, with <code>NSPT ≈ 1</code>, representing a very soft deposit like those found in the Amazon region.
    </p>
    <ul>
      <li><strong>HS-Small</strong> material model, calibrated with triaxial and oedometer tests.</li>
      <li>Refined triangular mesh near the load area.</li>
      <li>Used to <strong>visualize soil response</strong> under staged loading.</li>
    </ul>
  </div>

  <div style="flex: 1; min-width: 300px; text-align: center;">
    <img src="assets/model-sketch.svg" alt="Model geometry" style="width: 100%; max-width: 350px;">
  </div>

</div>

---

## 🟠 Undrained Plastic Stage

The first load increment is applied quickly, and the soil does not have time to drain. This causes:

- An **instant increase in pore pressure**
- **Plastic displacements** under the load
- **Effective stress drop**
- Changes in **stress orientation** and **shear zones**

**Pore Pressure Animation:**

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/LoadEng.mp4" type="video/mp4">
  </video>
</p>

**Undrained Displacement Animation:**

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/LoadMC_1_Eng.mp4" type="video/mp4">
  </video>
</p>

**Mohr Circles – Point A and B:**

- At **Point A** (beneath the load), pore pressure increases while total stress moves rightward, keeping effective stress nearly constant.
- At **Point B** (next to the load), stress directions rotate and both total and effective stress states evolve.

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/LoadMC_2_Eng.mp4" type="video/mp4">
  </video>
</p>

---

## 🔵 Consolidation Stage

After the undrained stage, the system is allowed to drain for a fixed period. During this time:

- **Pore pressures dissipate** gradually
- **Effective stresses increase**
- **Settlement continues** as volume change occurs
- The system transitions to a drained state

**Pore Pressure Dissipation Animation:**

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/Cons2_Eng.mp4" type="video/mp4">
  </video>
</p>

**Mohr Circles During Consolidation:**

- Effective stress grows as water drains.
- At the end of this stage, total and effective stresses converge (pore pressure = 0).

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/ConsMC_1_Eng.mp4" type="video/mp4">
  </video>
</p>

---

## 🟢 Safety Stage

After full consolidation, the model is tested for stability using the **strength reduction method** (SSR). In this stage:

- No excess pore pressure remains
- The **failure mechanism** becomes visible
- The **Factor of Safety (FoS)** is estimated by progressively reducing the strength parameters until collapse

**Failure Mechanism Animation:**

<p align="center">
  <video autoplay muted loop playsinline controls style="width: 100%; max-width: 100%;">
    <source src="assets/SSR.mp4" type="video/mp4">
  </video>
</p>

---

## 📌 Summary

This simplified example demonstrates how numerical models can be used not only to simulate real scenarios, but also to **gain intuition** about soil behavior under staged loading.

Numerical tools like PLAXIS, combined with scripting through Python, enable fast exploration of multiple scenarios and help us make better geotechnical decisions.

---



## 📚 About This Project

These animations were originally prepared for a technical talk at the  
**[V CIGEMIS – Congreso Iberoamericano de Geotecnia y Métodos Numéricos](https://sites.google.com/view/geogroup-uba/)**.

They are also used in the course **Geotecnia Numérica I**, part of the  
[**Specialization in Geotechnical Engineering**](https://www.fi.uba.ar/posgrado/carreras-de-especializacion/ingenieria-geotecnica)  
at the University of Buenos Aires (UBA).

You can access the source files and code used to generate these results in the  
[GitHub repository](https://github.com/ntasso/plaxis-animations).

<p align="left" style="display: flex; align-items: center; gap: 10px;">
  <img src="assets/profile.jpg" alt="Nicolás Tasso" style="width: 60px; border-radius: 50%; margin-right: 10px;">
  <a href="https://www.linkedin.com/in/ntasso" target="_blank">Connect with me on LinkedIn</a>
</p>
