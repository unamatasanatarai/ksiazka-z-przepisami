---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
tags: ["przepis"]
draft: true
---

# Przepis na {{ replace .Name "-" " " | title }}

- ⏲️  Czas przygotowania: 10 min
- 🍳 Czas gotowania: 30 min
- 🍽️ Liczba porcji: 4

opis

## Składniki

- abc

## Krok po kroku

1. a
2. b
