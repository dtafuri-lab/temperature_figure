# temperature_figure

I started this project from a simple observation — I kept checking the weather app before leaving the house but still ended up under or overdressed. The number on the screen never really translated into what to actually wear. So I wanted to make something physical that could do that for you.

**Week 1** was spent modelling the overall shape. I looked at how objects like pine cones respond to humidity changes and used that as a reference for something that reacts to its environment passively and visually.

**Week 2** I focused on the figure itself. The idea is a small human form whose arm moves to one of three positions depending on the temperature outside — jacket below 12°C, hoodie between 12 and 22°C, t-shirt above 22°C.

**Week 3** I worked out the twisting mechanism through the 3D model. The arm rotation is driven by a MG90S micro servo inside the body, controlled by a QT Py RP2040 that receives temperature data wirelessly from an ESP32-S3 placed outdoors via Bluetooth Low Energy.

The two units are self-contained and battery powered. This week the goal is to 3D print the parts, assemble everything, and get it running.

🔗 [github.com/dtafuri-lab/temperature_figure](https://github.com/dtafuri-lab/temperature_figure)
