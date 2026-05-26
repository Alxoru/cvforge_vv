<div align="center">

# 🔥 CVForge

**Собирай OpenCV-пайплайны как конструктор**

[![Python 3.10+](https://img.shields.io/badge/Python-3.10+-blue?logo=python)](https://python.org)
[![OpenCV 4.9+](https://img.shields.io/badge/OpenCV-4.9+-green?logo=opencv)](https://opencv.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

</div>

---

```python
# Было: 20 строк boilerplate
# Стало: 6 строк чистого кода

app = CVForgeApp(
    grabber=CameraGrabber(0),
    pipeline=Pipeline([
        GaussianBlurProcessor((5,5)),
        CannyEdgeProcessor(50, 150),
        AnnotateFPS(),
    ])
)
app.run("Edge Detection 🔍")
