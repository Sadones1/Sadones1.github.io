---
layout: project
type: project
image: img/FA.jpeg
title: "Freediving Adventures"
date: 2023-01-15
published: true
labels:
  - Freediving
  - Ocean
  - Community
summary: "Freediving Adventures is a project focused recording individual physical limits while building a community that fosters encouragement, saftey, and an environmentally sustainable mindset."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

A large part of freediving is physical but also mental wellness. A personal goal of mine is to dive further than 120 ft and a breathhold of 2 minutes. 
---

For this project, I was responsible for establishing the project and building the code to record the data. The events to collect the data would not have been possible without the amazing divers surround me. 

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
