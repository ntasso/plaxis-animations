# Clay Under Load – A Simple Visual Guide to Undrained, Consolidation and Safety Stages

This page is a visual explanation of what happens when a clay layer is loaded — and how these effects are captured in a PLAXIS numerical model through three common analysis stages:

- **Undrained Plastic**
- **Consolidation**
- **Safety**

---

## 🟠 Undrained Plastic Stage

A load is applied quickly on a soft clay layer. There's no time for drainage.

- Excess **pore pressures increase rapidly**
- **Displacements** occur, mostly from shearing
- **Effective stress drops**

**Pore Pressure Animation:**

<video controls style="width: 100%; max-width: 800px; display: block; margin: 0 auto;">
  <source src="assets/LoadEng.mp4" type="video/mp4">
</video>

**Undrained Displacement Animation:**

<video controls style="width: 100%; max-width: 800px; display: block; margin: 0 auto;">
  <source src="assets/LoadMC_1_Eng.mp4" type="video/mp4">
</video>

**Mohr Circles (Total & Effective Stress – Point A & B):**

<video controls style="width: 100%; max-width: 800px; display: block; margin: 0 auto;">
  <source src="assets/LoadMC_2_Eng.mp4" type="video/mp4">
</video>

---

## 🔵 Consolidation Stage

As time progresses, pore water drains and:

- Pore pressure **dissipates**
- Effective stress **increases**
- Volume change occurs, causing **further settlement**

**Pore Pressure Dissipation Animation:**

<video controls>
  <source src="assets/Cons2_Eng.mp4" type="video/mp4">
</video>

**Mohr Circles (during consolidation):**

<video controls>
  <source src="assets/Cons_MC_1_Eng.mp4" type="video/mp4">
</video>

---

## 🟢 Safety Stage

Once drained, the safety stage checks long-term stability.

- All excess pore pressures are gone
- We observe the **deformation mechanism**
- Factor of Safety is calculated

**Failure Mechanism (Safety Stage):**

<video controls>
  <source src="assets/SSR.mp4" type="video/mp4">
</video>

---

## 🔗 Source Files and Contact

- Code, files, and presentation: [GitHub repo](https://github.com/tuusuario/clay-staged-plaxis)
- For questions or collaboration: [LinkedIn Profile](https://linkedin.com/in/tuusuario)
