---
marp: true
theme: default
paginate: true
---

<style>
    h1{
        position: absolute;
        left: 50px; top: 50px;
    }
</style>

# 4.3.5 Probit regression

$$
\begin{aligned}

f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp{-\frac{(x-\mu)^2}{2\sigma^3}}
\end{aligned}
$$

$$
\Phi(a)=\int_{-\infty}^{a} \mathcal{N}(\theta \mid 0,1) \mathrm{d} \theta
$$
$$
\operatorname{erf}(a)=\frac{2}{\sqrt{\pi}} \int_{0}^{a} \exp \left(-\theta^{2} / 2\right) \mathrm{d} \theta
$$

$$
\boldsymbol{\Phi}(a)=\frac{1}{2}\left\{1+\frac{1}{\sqrt{2}} \operatorname{erf}(a)\right\}
$$

$$
\begin{aligned}
p(t \mid \mathbf{x}) &=(1-\epsilon) \sigma(\mathbf{x})+\epsilon(1-\sigma(\mathbf{x})) \\
&=\epsilon+(1-2 \epsilon) \sigma(\mathbf{x})
\end{aligned}
$$

---

# 4.3.6 Canonical link functions

$$
p(t \mid \eta, s)=\frac{1}{s} h\left(\frac{t}{s}\right) g(\eta) \exp \left\{\frac{\eta t}{s}\right\}
$$

$$
y \equiv \mathbb{E}[t \mid \eta]=-s \frac{d}{d \eta} \ln g(\eta)
$$

$$
y=f\left(\mathbf{w}^{\mathrm{T}} \boldsymbol{\phi}\right)
$$

$$
\ln p(\mathbf{t} \mid \eta, s)=\sum_{n=1}^{N} \ln p\left(t_{n} \mid \eta, s\right)=\sum_{n=1}^{N}\left\{\ln g\left(\eta_{n}\right)+\frac{\eta_{n} t_{n}}{s}\right\}+\text { const }
$$

---

$$
\begin{aligned}
\nabla_{\mathbf{w}} \ln p(\mathbf{t} \mid \eta, s) &=\sum_{n=1}^{N}\left\{\frac{d}{d \eta_{n}} \ln g\left(\eta_{n}\right)+\frac{t_{n}}{s}\right\} \frac{d \eta_{n}}{d y_{n}} \frac{d y_{n}}{d a_{n}} \nabla a_{n} \\
&=\sum_{n=1}^{N} \frac{1}{s}\left\{t_{n}-y_{n}\right\} \psi^{\prime}\left(y_{n}\right) f^{\prime}\left(a_{n}\right) \boldsymbol{\phi}_{n}
\end{aligned}
$$

$$
f^{-1}(y)=\psi(y)
$$

$$
\nabla \ln E(\mathbf{w})=\frac{1}{s} \sum_{n=1}^{N}\left\{y_{n}-t_{n}\right\} \phi_{n}
$$

---
<style scoped>
  section {
    font-size: 400%;
  }
</style>

aaa
<span style="color:red">a<span>
