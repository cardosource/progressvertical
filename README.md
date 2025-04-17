# 📊 ProgressVertical

**ProgressVertical** é uma biblioteca Python **em desenvolvimento** para a exibição de barras de progresso **verticais** em aplicações de linha de comando (CLI).

Projetada com foco em **usabilidade** e **personalização**, permite criar animações de progresso multi-etapas com:
- Cores e estilos configuráveis
- Duração ajustável
- Inspiração na biblioteca [progressbar](https://pypi.org/project/progressbar/)

**Dinamismo e clareza visual**!

---

ㅤ <img src="https://cdn.pixabay.com/photo/2025/04/14/20/46/20-46-21-815_960_720.png" alt="Fluxograma" width="500" height="250" />

---

### 📦 Instalação

> pip install progressvertical


## Exemplos de Uso
Exemplo 1 – Múltiplas listas com rótulos e barras de colores diversificadas.

```python
from progressvertical import ProgressManager, VerticalProgressRenderer, ColorManager

ColorManager.init_colorama()
renderer = VerticalProgressRenderer(height=5,spacing=5)
manager = ProgressManager(renderer)

name_list = ["Mel", "Bianca", "Melissa","Piqueno","Netuno","Merenga"]
numbers_list = [10, 20, 30, 40, 50]
color_list = ["vermelho", "verde", "azul", "amarelo"]


print("starting")

for name in manager.track(name_list, label="Names", fore_color="ciano"): __import__('time').sleep(0.4)
for number in manager.track(numbers_list, label="Number", fore_color="verde"): __import__('time').sleep(0.3)
for color in manager.track(color_list, label="Color", fore_color="magenta"): __import__('time').sleep(0.2)
print("finished")
 


```




[![📊 ProgressVertical](https://img.shields.io/badge/📊%20ProgressVertical-%200.2.2-0073B7?style=for-the-badge)](https://pypi.org/project/progressvertical/)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
