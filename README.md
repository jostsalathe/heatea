# heatea

For now just kicking around concepts:

## Notes applying to all designs

- The heating element shall have a heat transferring surface with at least 110 mm diameter.
- A hexagonal hot plate outline would make building a wood enclosure more easy.
- The power input for the heating element shall use USB C power delivery

## Self designed heating pcb

- The PCB shall have a heating track on the top side.
- The heating track shall have about 100 W of heating power at 20 V to get the most power out of the USB PD spec.
- The PCB shall have its power circuitry on the bottom side.
- The necessary PD controller shall be configurable to request different voltages so that the user can effectively select output power.

## Aluminium hot plate

- The hot plate shall be an aluminium disk like this: [Aluminum Circular Plate, Aluminum disc, With a Diameter of 150mm And a Thickness of 4.0mm](https://www.aliexpress.com/item/1005006307340025.html).
- heated by one of
    - (Dia 120mm 50W Round Circular Silicone Heater HeatBed Heating Pad with Thermistor Delta kossel 3D Printer parts)[https://www.aliexpress.com/item/1005005868301433.html] (only 50W...)
    - (AC/DC 24V Max 150W Egg Incubator Heater Aluminum PTC Heater Heating Element Thermostat Heater Plate 77*62*6mm)[https://www.aliexpress.com/item/32696928363.html] maybe complemented by (10K B3435 M4 Surface Fixed NTC Thermistor Negative Temperature Coefficient Probe Line Ear 30CM)[https://www.aliexpress.com/item/1005006370359527.html] (more work to mount it...)
- This design shall include a temperature controller.
- The temperature controller shall be implemented on a microcontroller.
- The microcontroller shall read the temperature probe of the heating element.
- The microcontroller shall switch the heating element via a MOSFET according to the control scheme.
- The microcontroller shall be able adapt the requested supply voltage from the USB PD controller.
