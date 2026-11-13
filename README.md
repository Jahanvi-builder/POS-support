# POS guided help — clickable prototype

A clickable prototype of the guided "Log a complaint" flow for the POS payments app: the merchant picks what's wrong, the device runs a check, tries a fix, and only then offers to raise a request.

It is a design prototype. Nothing is connected to a real device or backend; check results are simulated, and values such as phone numbers, request numbers and call-back times are placeholders.

## Run it

Open `index.html` in a browser. There is no build step and no dependencies (the Inter font loads from Google Fonts).

## Host on Vercel

1. Import this repository at vercel.com/new.
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy. `index.html` is served at the root.

## What's built

- Power and charging: won't charge, battery runs out fast, battery swollen or hot
- Screen and buttons: touch test, slow screen fix ladder, cracked screen
- Request: registered or different number (number pad and code), raised, failed, open-request check

Greyed options are not built. The panel beside the phone sets what the simulated checks find.

## Editing

Everything is in `index.html`: the screen markup is in the `<template id="tpl">` block, and the flow logic is the `Component` class in the script below it.
