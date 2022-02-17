---
marp: true
theme: default
paginate: false
---

<style>
    h1{
      position: absolute;
      left: 50px; top: 50px; bottom:50px;
    }
    .split {
      display: table;
      width: 100%;
    }
    .split-item {
      display: table-cell;
      padding: 0px;
      width: 60%;
    }
    .split-left {
      position: relative;
    }
    .split-left__inner {
      height: 100%;
      position: fixed;
      width: 50%;
    }
    .split-right {
      position: relative;
    }
    .split-right__inner {
      height: 420px;
    }
</style>



<style scoped>
  section {
    font-size: 140%;
  }
</style>

<div class="split">
  <div class="split-item split-left">
    <div class="split-left__inner">

- 以下のQUBO形式のベイズ線形回帰モデルを <span style="color:red">獲得関数</span> としたBBO手法
  $$ \tilde{f}(\vec{\bm{x}}\mid\vec{\bm{\alpha}}) = a_0 + \Sigma_{i}a_i x_i + \Sigma_{i < j} a_{ij} x_i x_j$$
- 離散変数を含むBBOに対するベイズ最適化手法として提案されている

    </div>
  </div>
  <div class="split-item split-right">
    <div class="split-right__inner">

  $$ \tilde{f}(\vec{\bm{x}}\mid\vec{\bm{\alpha}}) = a_0 + \Sigma_{i}a_i x_i + \Sigma_{i < j} a_{ij} x_i x_j$$

    </div>
  </div>
</div>

---
