# Ghostbusters Atari Clone - Implementation Plan

## 1. Engine Setup
- HTML5 Canvas @ 320x200 (scaled for modern screens).
- State Machine: `TITLE`, `SHOP`, `CITY_MAP`, `DRIVING`, `CAPTURE`, `GAME_OVER`.
- Atari Palette mapping.

## 2. Shop System (Sistema de Economia)
- Initial Balance: $5000.
- Items:
    - Image Sensor: Detects ghosts on map early.
    - Ghost Vacuum: Used in driving sequence to prevent PK increase.
    - Extra Traps: Increases capacity.

## 3. Map Logic (Mapa de Navegação)
- 8x8 City Grid.
- Ghost icons moving toward "Ghostbusters HQ" (Center).
- Flashing buildings (Emergencies).
- Ecto-1 icon movement.

## 4. Driving Sequence (Sequência de Direção)
- Side-scrolling road.
- Vacuum ghosts to prevent PK Meter rise.
- Ecto-1 movement up/down.

## 5. Capture Sequence (Captura de Fantasmas)
- Two Ghostbusters sprites.
- Proton beam animation (zigzag line).
- Trap placement logic.
- Ghost AI (erratic movement).

## 6. Resource Management (Gestão de Recursos)
- PK Meter tracking.
- Backpack Energy during capture.
- Trap count.

## 7. Win/Loss Condition (Condição de Vitória/Derrota)
- PK Meter reaching 9999 leads to Stay Puft and Game Over.
- Money accumulation tracking.

## Technical Details:
- Pure JS/Canvas (No external assets).
- Web Audio API (Atari-style synthetic sounds).
- Atari 2600 NTSC Palette.
