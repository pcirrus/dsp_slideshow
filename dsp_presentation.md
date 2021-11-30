---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.13.2
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

+++ {"slideshow": {"slide_type": "slide"}}

# Analiza sygnału

- Proces *wyciągania* informacji z określonego sygnału nazywa się **analizą sygnału**.
- Najczęściej przeprowadza się **analizę czasową** oraz **analizę częstotliwościową**

```{note}
Test
```

```{figure} ./img/ecg_normal_public_domain.jpg
---
align: center
name: normal-ecg
---
Ilustracja normalnego, 12-odprowadzeniowego EKG (Glen Larson, Wikimedia Commons)
```


```{code-cell} ipython3

```

+++ {"slideshow": {"slide_type": "slide"}}

# Sposoby analizy czasowej
- badanie wartości
- interpolacja
- autokorelacja
- segmentacja

+++ {"slideshow": {"slide_type": "slide"}}

# Analiza częstotliwościowa

**Częstotliwość** - powtarzalność zjawiska w określonej jednostce czasu

Wiele sygnałów ma komponenty powtarzające się w czasie:
- sygnały zmodulowane
- fale akustyczne i radiowe
- i inne

+++ {"slideshow": {"slide_type": "subslide"}}

Większość sygnałów określonych jest w dziedzinie czasu: **f(t)**

**TODO: spektrogram sygnału audio**

Jak przekształcić *sygnał zależny od czasu* w *sygnał zależny od częstotliwości*?

+++ {"slideshow": {"slide_type": "subslide"}}

# Rozwiązanie - funkcje trygonometryczne!

- sin(x) - ma częstotliwość 1 Hz
- sin(2x) - częstotliwość 2 Hz
- sin(nx) - częstotliwość n Hz

**Gdyby tylko dało się wyrazić naszą funkcję za pomocą sumy wielu sinusów!**

+++ {"slideshow": {"slide_type": "subslide"}}

## Szczęście w nieszczęściu

**TODO**
- wyjaśnić przestrzeń liniową i bazę
- pokazać bez dowodu że szereg Fouriera jest bazą
- i że z twierdzenia Eulera-Fouriera możemy wyrazić sporą część funkcji w ten sposób

+++ {"slideshow": {"slide_type": "subslide"}}

**Tutaj przykłady transformacji Fouriera**

+++ {"slideshow": {"slide_type": "subslide"}}

# Idźmy dalej...

**dyskretna transformata Fouriera**

+++ {"slideshow": {"slide_type": "subslide"}}

# Złożoność obliczeniowa

**FFT - Cooley-Tukey**

+++ {"slideshow": {"slide_type": "subslide"}}

# Własności transformaty Fouriera

**TODO**
- splot -> mnożenie
- odwrotna transformata Fouriera

+++
