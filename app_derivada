import streamlit as st
import numpy as np
import matplotlib.pyplot as plt

# Título de la aplicación
st.title("Gráfico de una Función Convexa y su Derivada")

# Valor inicial de la derivada
initial_derivative = st.slider("Valor de la Derivada", min_value=-5.0, max_value=5.0, value=1.0, step=0.1)

# Generar datos de la función convexa y su derivada
x = np.linspace(-10, 10, 400)
y = x**2  # Función convexa (x^2)
derivative = 2 * x  # Derivada de la función (2x)

# Actualizar la derivada con el valor del slider
derivative = initial_derivative * x

# Crear el gráfico
fig, ax = plt.subplots()
ax.plot(x, y, label="Función Convexa (x^2)")
ax.plot(x, derivative, label=f"Derivada (2x * {initial_derivative})", linestyle="--")
ax.legend()

# Mostrar el gráfico en Streamlit
st.pyplot(fig)
