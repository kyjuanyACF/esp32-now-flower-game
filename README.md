# Multiplayer Plant Game
 
Made collaboratively by Kyjuany Cintron & Tiffany Yaxi Tu
 
A two-player button smashing game for the ESP32. One player adds water, the other adds sunlight, so together you grow a plant from a seed to a flower.
 
[Full documentation](https://kyjuanyacf.github.io/creative_embedded_systems/)
 
## How it works
 
- One board is **water**, the other is **sunlight**
- Press your buttons to add your resource
- The plant only grows as much as the lower resource, so you need both players pressing buttons
- Hit 20 presses each and the flower blooms 
- Press again to start over as a seed

The boards send each other their press counts using ESP-NOW, so both screens show the same plant.

## Hardware
- LilyGO TTGO T-Display (ESP32 with a 240×135 screen)
- USBC cable
  
## Run it yourself!
 
1. Install the ESP32 board package and the TFT_eSPI library in Arduino IDE
2. In the code, set `PLAYER_ID` to `0` on one board and `1` on the other
3. Keep `TEAM_ID` the same on both boards
4. Upload to both boards and start pressing buttons!
   
## How it works
 
