# YACoVV - Yet Another (SARS-)CoV(-2)Ventilator

[German-Version is more Detailed / updated more frequently](README_DE.md) <- Please translate (see Contributing)!

This project aims at constructing components for the production of ventilators that can be used as last-resort-solutions for SARS-CoV-2 patients. 

All components should be constructed with parts, raw materials and skills needed in the places in which the devices come into use. 

The most complex component of a ventilator is the correct, reliable and safe pressure control of the ventilator as well as keeping the positive end-expiratory pressure intact. Currently, there is a promising solution for the pressure control that has already been transferred into a functioning sample.

The components are:
- [Pressure regulator and timing](#Pressure%20regulator)
    - Regulation of the ventilation pressure
    - Upholding the modifiable PEEP
    - Regulation of modifiable I:E relation
- [Respiratory gas/ Processing](#Breath%20gas%20production)
    - ozone/oxygen mixture
    - Recovery
        - Co2-absorber 
    - Heating 
    - Humidification
- [Monitoring](#Monitoring)
    - Measurement of volume
    - Measurement of pressure
    - Measurement of frequency

[miro-Board](https://miro.com/app/board/o9J_kuxCsRI=/) (Idea and Link Collection)

## Pressure regulator
### Here’s a video of a prototype
https://www.youtube.com/watch?v=eBIlyaHW4l0

Problems with this prototype:
- [Lack of check valves](https://github.com/auenkind/YACoVV/issues/3)
- [Air bubbles in discharge hose too big](https://github.com/auenkind/YACoVV/issues/1)
- [Servo/Microtroller](https://github.com/auenkind/YACoVV/issues/2)

### Functional principle
The concept behind the water column makes sure pressure regulation functions. To generate modifiable pressures in the system, tubes are immersed into water appropriate to the wanted pressure. The control tubes are simultaneously used as relief valve. 

The “return paths” of the water column are savely secured through check valves so that no water can flow back to the patient.

Because the high entrance pressures can only be regulated through this system with very precise component rules, we decided on using a 50 mBar gas pressure regulator to pre-regulate the pressure. Since these regulations are available all over the world, they are an ideal solution for our problem.

We are using the basic principle behind constriction hose-valves for our valves since these can be easily manufactured out of widely available components. On top of that, these kinds of valves bear the advantage that all components that come into contact with contaminated gas can be replaced. 

#### Valve-Control and Timing

The timing currently functions through a microcontroller and two servos. This solution will replaced with the motor of a windscreen wiper with two camdiscs.

![Camdiscs](img/camdisc.png)

[Camdisc Animation](https://autode.sk/3dx6EbZ)

#### Inhalation
![inhalation](img/insp.png)
#### Exhalation
![exhalation](img/exp.png)

## Breath gas production
This component reuses the exhaled breath gas. Co2 is absorbed and oxygen is mixed in. 

## Monitoring
This component supervises the pressure level, the pressure swing and frequency during ventilation.

## Contributing
We are happy about every contribution to this project! We need action NOW! Please don’t overthink your contribution, join us!

If these projects’ solutions win prizes in competitions such as the [Code Life Ventilator Challenge](https://www.agorize.com/en/challenges/code-life-challenge?lang=en), we will use the money to construct the components or improve the design.

Things everyone can do:
- Translation of the README_DE.md in as many languages as possible. Translations will have be adjusted very frequently, changes should quickly be translated.
- Construct a YACoVV und run it! Feedbacks on the materials used and problems that have come up would be awesome!
- Take on one of the concrete problems in the issue section.