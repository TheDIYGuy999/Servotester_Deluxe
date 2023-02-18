# Servotester_Deluxe

The original autor is "Der RC Modellbauer": https://www.youtube.com/@DerRCModellbauer

forked from his GitHub: https://github.com/Ziege-One/Servotester_Deluxe

PCB, schematic and more details: https://www.pcbway.com/project/shareproject/Servotester_Deluxe_62a3f47c.html

## New in v0.9.0:
- Servo is able to oscillate way faster in automatic mode, speed adjustability improved
- Made sure, there is no language string array pointer overflow, if EEPROM was deleted before
- There are still issues with unstable Multiswitch readings. Solution for now: use the pre compiled bin files or use Arduino IDE 2.0.3 with espressif board 2.0.5 (which is unfortunately incompatible with VS Code)

## New in v0.8.0:
- Support for calibrated analogRead, using the ESP32AnalogRead library is improving battery monitoring
- Number of LiPo battery cells is displayed
- Message, if no valid battery is detected
- Support for French language added

## New in v0.7.1:
- ESPHome-Flasher discovered a serious EEMPOM bug, because flash is erased before upload. It should now be fixed.

## New in v0.7.0:
- It is now compatible with VS Code / Platformio. This makes board and library version management way easier, because all is defined in platformio.ini and downloaded automatically. Of course it is still compatible with Arduino IDE
- No external SBUS library required anymore
- Adjustable WiFi power
- Support for alternative logo
- New menu options: 
-- Encoder direction inversed or not
-- SBUS inversed or not
-- Language English or German (others could easily be added)
-- Help text is displayed during start
