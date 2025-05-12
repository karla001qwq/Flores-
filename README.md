import matplotlib.pyplot as plt
import numpy as np

# Definir el ángulo dorado
golden_angle = 137.5077640500378546463487396283702776206886952699253696312384958261062333851951
phi = golden_angle * np.pi / 180

# Calcular las coordenadas x e y de cada flor
n = 1000
theta = np.arange(n) * phi
r = np.sqrt(np.arange(n))

x = r * np.cos(theta)
y = r * np.sin(theta)

# Graficar el girasol
plt.figure(figsize=(8, 8))
plt.scatter(x, y, s=10, c='yellow', alpha=0.5)
plt.axis('equal')
plt.axis('off')
plt.show()
