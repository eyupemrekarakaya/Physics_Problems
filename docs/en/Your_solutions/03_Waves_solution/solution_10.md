## 10. Animation: Wave Sources

Wave equation:

$$
u(\vec{r}, t) = \frac{A}{|\vec{r} - \vec{r}_0|^\alpha} \sin(k|\vec{r} - \vec{r}_0| - \omega t)
$$

---

### Description

- $\vec{r}_0$ → source position  
- $\alpha \in [0,2]$ controls amplitude decay  
- Each point acts as a wave source  

---

### Superposition

Total wave from multiple sources:

$$
u_{\text{total}} = \sum_i \frac{A}{|\vec{r} - \vec{r}_i|^\alpha} \sin(k|\vec{r} - \vec{r}_i| - \omega t)
$$

---

### Key Concepts

- Waves spread radially  
- Amplitude decreases with distance  
- Multiple sources → interference patterns  

---

### Final Idea

Wave field is obtained by summing contributions from all sources:

$$
\boxed{u(\vec{r}, t) = \sum_i u_i(\vec{r}, t)}
$$
