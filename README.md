---
title: "JD→CV Matcher"
emoji: "🧭"
colorFrom: "indigo"
colorTo: "blue"
sdk: gradio
sdk_version: "4.27.0"
app_file: app.py
pinned: false
license: mit
---
# JD→CV Matcher

Analiza tu CV frente a una oferta de empleo (JD) y entrega:
- Score de match (0–100)
- 5 mejoras concretas del CV
- 1 bullet optimizado (formato STAR, con métricas)
- Palabras clave faltantes
- Resumen sugerido (2–3 frases) adaptado al JD

- Gratis: 3 usos/día
- Pro: ilimitado ($7–$9)

Enlaces:
- Space (usar ahora): https://huggingface.co/spaces/luisarli/JD-CVMatcher
- Comprar licencia Pro (Gumroad): https://aiarepita.gumroad.com/l/fxfvva

![Demo](./demo.gif) <!-- Reemplaza cuando subas tu GIF -->

## Cómo usar

1) Abre el Space: https://huggingface.co/spaces/luisarli/JD-CVMatcher  
2) Pega la Oferta (JD) y tu CV en texto.  
3) Opcional: pega tu Clave Pro (si la adquiriste en Gumroad) para uso ilimitado.  
4) Haz clic en “Analizar”.

La app devuelve:
- Score de match
- 5 mejoras accionables
- Un bullet optimizado (STAR + métricas)
- Keywords faltantes
- Un resumen breve adaptado al JD

## Pro (Licencias)

- Compra tu licencia en Gumroad: https://aiarepita.gumroad.com/l/fxfvva  
- Tras la compra, recibirás una clave (ej: `ABCDEF-123456-2025`).  
- La app valida la clave contra un JSON público de licencias (MVP simple).  
- Si tu clave está en la lista, se desbloquea el uso ilimitado (sin límite diario).

> Nota: Validación sencilla pensada para MVP. No expone datos personales y se puede reforzar más adelante (webhooks, tokens firmados).

## Tecnologías

- UI/hosting: Hugging Face Spaces (Gradio)  
- LLM: OpenAI `gpt-4o-mini` (configurable)  
- Licencias: JSON público (validación ligera)

## Privacidad

- No almacenamos texto de JD/CV.  
- El contador de usos se mantiene en memoria de sesión del Space.  
- Puedes borrar tus contenidos del input en cualquier momento.

## Roadmap

- Exportar “Match Report” a PDF (1 página).  
- Modo “ATS-friendly rewrite”.  
- Detección automática ES/EN y respuesta en el idioma del input.  
- Batch para múltiples JDs (solo Pro).  
- Explicabilidad del score (mostrar pesos por dimensión).

## Contribuir / Feedback

- Abre Issues con sugerencias o problemas.  
- Comparte antes/después de bullets optimizados (anónimo) para mejorar prompts.

## Licencia

MVP educativo. Uso bajo tu responsabilidad. © TuNombre
