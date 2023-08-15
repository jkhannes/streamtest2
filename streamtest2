import streamlit as st
import numpy as np
import matplotlib.pyplot as plt

st.title("Einfache Streamlit App")

# Texteingabe
name = st.text_input("Geben Sie Ihren Namen ein:", "Max")

# Zahleneingabe
number = st.number_input("Geben Sie eine Zahl ein:", 0, 100, 50)

st.write(f"Hallo {name}! Sie haben die Zahl {number} eingegeben.")

# Interaktiver Plot
st.subheader("Interaktiver Plot")

x = np.linspace(0, 10, 100)
y = np.sin(number * x)

fig, ax = plt.subplots()
ax.plot(x, y)
ax.set_xlabel("X-Werte")
ax.set_ylabel("Y-Werte")
ax.set_title("Sinus-Funktion")

st.pyplot(fig)

# Checkbox
show_data = st.checkbox("Daten anzeigen")
if show_data:
    st.write("Hier sind einige Beispiel-Daten:")
    st.dataframe(np.random.randn(5, 5), columns=["A", "B", "C", "D", "E"])

# Auswahlbox
option = st.selectbox("Wählen Sie eine Option aus:", ["Option 1", "Option 2", "Option 3"])
st.write("Sie haben die Option ausgewählt:", option)
