## Modelling building energy performance

It is suprisingly straighforward to gain significant insight into a buildings energy performance, such as working out how much heating energy it should require to keep it at 20C for a year by doing a little math. This guide walks through how to do these calculations starting with a simple model and advancing through to a full SAP model and beyond to some very simple dynamic simulation.

The guide is currently a work in progress, if you'd like to help get in contact

The following diagram illustrates the most common factors taken into account in building energy models:

![diagram.png](files/diagram.png)


### Part 1: Heat losses

- Conduction through building fabric: walls, windows, loft, floor, thermal bridges. Calculated via material U-values or thermal conductivity.
- Ventilation and Infiltration

### Part 2: Internal gains

- Metabolic (body heat)
- Lighting
- Appliances
- Cooking
- Hot water, including solar hot water
- Heating system

### Part 3: Solar gains

### Part 4: Further considerations

- Utilisation factors of gains
- Thermal mass

### Model types

For examples of the following model types see the model [examples page](modelexamples.md).

**Simple annual**
The simplest of all models, possible to get good insight into energy performance with the least amount of calculations, but not as accurate as more detailed models.

**Simple monthly**
A very common simple model type, used in SAP and PHPP, more accurate than the annual model and gives insight into seasonal factors throughout a year. Require's higher detail datasets.

**Simple daily**
As above but on a daily basis

**Dynamic simulations**
The simple model's use averaged annual, monthly datasets and so give outputs that are averages for a year/month. Dynamic simulations can give far greater detail and can be useful for finding out what happens in extremes of climate: hour-by-hour on a sunny day in June rather than the average for June. 