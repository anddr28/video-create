# Промпты по планам

Общий префикс (добавлять в начало каждого плана):

```
Vertical 9:16, 1080x1920, photorealistic 4K product commercial, cinematic tabletop
cinematography. Camera at object height, tilted down 5–10 degrees, smooth slider-like
motion, zoom no more than 10–15% per shot, no shake. No on-screen text, no graphics,
no people or faces (hands only where stated).

PRODUCT (identical in every shot, match the reference image exactly): clear plastic
1000 ml bottle filled with clear liquid, red ribbed screw cap. White label with a dark
navy block, centered text top to bottom: red "А" and blue "Х" logo; "АЛЬФАХИМИЯ" in
navy Cyrillic capitals; "ЭТИЛОВЫЙ СПИРТ" in large white letters on navy; "96%" in very
large white digits on a red band; "ЧИСТОЕ ГОРЕНИЕ" small, with a navy flame icon below;
"1000 мл" at the bottom. Crisp, sharp, correctly spelled Russian Cyrillic, stable and
undistorted. The bottle is always fully in frame, no taller than 60% of the frame
height, never cropped, never rotated.
```

## План 1 — Продукт (0–3 с, генерировать 4 с)

Стартовый кадр: бутылка из `assets/bottle_reference.png` справа, спиртовка слева, светлый лабораторный стол.

```
Medium shot on a bright modern laboratory bench, soft daylight, creamy bokeh of glassware
in the background. Right: the 1000 ml bottle standing upright, label facing camera.
Left: a glass alcohol lamp with a brass burner and cotton wick, its brass cap on a small
chain beside it. A hand in a white lab-coat sleeve lifts a second identical bottle and
carefully pours a thin stream of clear liquid into the alcohol lamp, no spills.
Camera slowly trucks right. The bottle on the right stays fully visible with readable label.
```

## План 2 — Пламя (3–6 с, генерировать 4 с)

```
Medium shot, same laboratory bench. The alcohol lamp wick ignites with a soft flash and
settles into a steady clean flame: blue at the base, golden at the tip, no smoke, no soot.
Gentle slow push-in (under 10%).
```

Второй клип для растворения (2 с):

```
Outdoors at dusk, on dark rocks with soft forest bokeh. A compact alcohol camping stove
burns with a ring of blue flame; a brushed steel camping mug sits on it, light steam
rising. Slow lateral slider move. Warm and cool dusk light, no smoke.
```

## План 3 — Финал (6–10 с, генерировать 4–5 с)

Стартовый кадр: бутылка строго по центру, этикетка фронтально; спиртовка рядом слева.

```
Frontal medium shot in the bright laboratory. The 1000 ml bottle stands fully in frame at
center, label facing straight to camera and perfectly legible. Next to it the alcohol lamp
burns with a steady blue-and-gold flame. Warm flame highlights reflect on the bottle's
plastic. Camera almost static, very subtle push-in (no more than 10%). Calm, clean, premium.
```

## Монтаж

- 0.0–3.0 — План 1.
- ~3.0 — склейка по вспышке: 4–6 кадров белого/тёплого flash, переход на загорание фитиля.
- 3.0–4.6 — пламя спиртовки; 4.6–6.0 — растворение (cross-dissolve ~0.5 с) в походную сцену.
- 6.0 — cross-dissolve ~0.5 с в План 3; 6.0–10.0 — финал, последняя секунда без речи.
- Экспорт: H.264/H.265, 1080x1920 (или 2160x3840), 30 fps, без титров.
