---
title: ♥ Hardware for Good
type: about
---

Hello! And welcome to the documentation website for **EC.751 / EC.793 (G) Hardware Design for the Developing World**! This class is focus on applying the concepts of upcycled electronics, electrical design, remote sensing and monitoring, and mechatronics to problems related to the [UN Sustinable Development Goals ↗](https://sdgs.un.org/goals) with D-Lab partners around the world. This includes exploring applications to health, energy, education, and agriculture to have a positive impact on people living in low-income and under-served communities around the world. This class is offered in conjunction with the MIT D-Lab program [Design for Second-Life Innovations ↗](https://d-lab.mit.edu/innovation-practice/design-second-life-innovations).

<div class="mt-6"></div>

{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="Heewon Lee"
    subtitle="Instructor, Research Scientist, MIT D-Lab"
    link="mailto:heewon1@mit.edu"
  >}}
  {{< hextra/feature-card
    title="Adi Mehrotra"
    subtitle="Instructor, MIT D-Lab; Researcher, MIT Department of Mechanical Engineering"
    link="mailto:adim@mit.edu"
  >}}
{{< /hextra/feature-grid >}}

See the link below for a PDF of the syllabus!

<div class="mb-6"></div>
{{< hextra/hero-button text="Course Syllabus, Spring 2024" link="docs" >}}

<div class="mt-6"></div>

## Contents of this Website

Please note that if you're an actively enrolled student **you must also have access to the canvas website to recieve announcements, submit assignments, and more.** We will be using canvas for managing grades, assignments, and general course logistics. This site is focused on documentation.

As you will be creating complex mechatronics systems with your community partners abroad, it's essential you and your partners both have access to adequate technical information to build your skillsets together. This website was designed to consolidate the hardware and software documentation required for the course in a place where both you and your community partners can access it easily. This includes the following:

- Basic information on using sensors, actuators, arduino and the arduino cloud, connecting with smartphones, and data management. 
- Considerations on designing electronic systems for remote environments.
- Consolidated readings on electrical design, safety, and mechatronics. 
- Links to great educational resources including textbooks, youtube channels, free software, and other courses.
- Public documenations on the labs and tutorials.

Additionally, the content on this website is [released open-source under creative commons ↗.](https://creativecommons.org/licenses/by/4.0/) So it can be shared with anyone! 

<div class="mt-6"></div>

## Combining Design and Technical Education

This is a unique class for both MIT as well as D-Lab because of our focus on combining two, generally independent streams of though to build robust products for harsh environments while considering our users needs, and socioeconomic contexts. We call it **technically rigorous product design for developing contexts.** 

Here's what the product design process generally looks like. It's a little messy, but there's always a lot of feedback:

```mermaid
graph TD;
    id1["Problem Framing, User Interviews"];
    id2["Needs Assessment"];
    id3["Ideation"];
    id4["Sketch Modeling"];
    id5["Prototyping"];
    id6["Looks Like"];
    id7["Works Like"];
    id8["Tests Like"];
    id9["User Feedback"];
    id10["Field Testing"];
    id11["High-Fidelity Prototype + Scaling"];
    id1-->id2;
    id2-->id3;
    id3-->id4;
    id4-->id5;
    id5-->id6;
    id5-->id7;
    id5-->id8;
    id6-->id9;
    id7-->id9;
    id8-->id9;
    id4-->id9;
    id9-->id4;
    id9-->id5;
    id9-->id11;
    id11-->id10;
    id10-->id11;
```

And here's what the engineering design process generally looks like (see [FUNdaMENTALs of Design by Alex Slcoum ↗](https://meddevdesign.mit.edu/fundamentals-downloads/?eeFolder=FUNdaMentals-Chapters)). It's also worth looking at the [NASA Technology Readiness Levels (TRLs) ↗](https://www.nasa.gov/directorates/somd/space-communications-navigation-program/technology-readiness-levels/):

```mermaid
graph TD
    id1["Functional Requirements"];
    id2["Environment Ergonomics"];
    id3["Design Parameters"];
    id4["Analysis"];
    id5["References"];
    id6["Risks"];
    id7["Countermeasures"];
    id8["Verification of Theory in Hardware Experiments"];
    id9["Small Scale Prototyping"];
    id10["Reliability, Lifetime, and Degradation Tests in the Appropriate Environment"];
    id11["Full Scale Prototype Engineered for Reliability"];
    id12["Field Testing"];
    id1-->id2;
    id2-->id3;
    id3-->id4;
    id4-->id5;
    id5-->id6;
    id6-->id7;
    id7-->id1;
    id7-->id8;
    id8-->id9;
    id9-->id10;
    id10-->id11;
    id11-->id12;
    id8-->id4;
    id9-->id1;
    id12-->id11;
    id10-->id8;
    id2-->id10;
```

In this class we're going to combine these two processes into one, and also apply it to mechatronics / IoT systems in developing world contexts. We're still developing this concept, but that process is going to look something liks this.

```mermaid
graph TD
    id0["Project Selection"];
    id1["Socioeconomic Problem Framing"];
    id2["Partner Needs Asessment"];
    id3["Technical System Requirements"];
    id4["Functional Block Diagram"];
    id5["Ideation/Idea selection"];
    id6["Sketch Modeling"];
    id7["System Architecture Design"];
    id8["User Feedback & Design Review 1"];
    id9["Prototyping"];
    id10["Works Like / System-on-Bench"];
    id11["Looks Like / Integration Tests"];
    id12["Peer Review / User Feedback / Design Review 2"];
    id13["High Fidelity Prototype"];
    id14["Field Testing in Appropriate Environment"];
    id15["Project Documentation"];
    id0-->id1;
    id1-->id2;
    id1-->id3;
    id3-->id4;
    id2-->id5;
    id5-->id6;
    id4-->id7;
    id7<-->id8;
    id6<-->id8;
    id8-->id9;
    id9-->id10;
    id9-->id11;
    id7-->id10;
    id6-->id11;
    id11-->id12;
    id10-->id12;
    id12-->id13;
    id13-->id14;
    id14-->id13;
    id14-->id15;
```

<div class="mt-12"></div>

## Class FAQ

{{% details title="Cross Registration" %}}

If you attend either Harvard or Wellesley, you **may cross register for this class.** Please check with your specific school/department on instructions for cross registering, and please email the instructors to check class avaliability! 

{{% /details %}}

{{% details title="Technical Level of this Course" %}}

Note that this course is *designed to teach you technical content,* so not having a background in electronics does not necessarily disqualify you from taking this course. However, it is important to note that this class is technical, and we will be posting a number of resources for you to take advantage of to get up to speed on the technical content. However, a short list of things to become familiar with before taking the course might be:

- Arduino wiring and programming (basic)
- Introductory electronics, ohm's law, KVL, KCL, voltage and current rating of components, series and parallel combinations
- Basic circuit components, voltage dividers, potentiometers, transistors, op-amps, ADCs/DACs, relays

**Don't be scared! We will post a number of resources for you to get caught up on these!**

**Advanced content.** Please note that if you're a student that has ample experience in electrical design, this course is STILL worth taking. We want to offer resources that help you learn considerations for designing electrical systems for developing contexts. This includes PCB design, selecting components to avoid supply chain issues, selecting components to minimize cost while maintaining robustness and functionality, and more. Please email us for more info! 

{{% /details %}}

{{% details title="🔧 Fabrication and Prototyping" %}}

Please note that as of the 2024 Spring version of this course, we do not currently have access to the D-Lab shop. This is due to high demand, and because this class is running as a pilot program for the first semester. Please let your instructors know if you have fabraction needs that include 3D Printing, Welding, CNC Machining, or other forms of fabrication ASAP so we can get you access to the right resources. **Please note that shop safety training is your responsibility for 2024.**

{{% /details %}}

{{% details title="⚠ Safety" %}}

We take safety in this class seriously, especially in the world of electronics. Note that according to OSHA, most electrical systems under 50V DC are considered safe to use with minimal precautions. However, we may exercise increased precaution in this class beacuse some students may be less familiar or comfortable around electronics systems. **Our policy, in general, is if you're unsure please ask before doing anything. Electronics is hard, and unintuitive, so it's better to ask than to hurt yourself.**

{{% /details %}}

<div class="mt-12"></div>

## Special Thanks To

Special thanks goes to Libby McDonald, Nancy Adams, Libby Hsu, Ana Pantelic, Dan Sweeney, and the rest of the amazing people at MIT D-Lab. An additional thank-you goes out to our community partners Twende (Tanzania), Kulika Uganda, and Youth Social Advocacy Team (Uganda, South Sudan). Finally, a special thanks goes to the [Korean International Cooperation Agency (KOICA) ↗](https://www.koica.go.kr/koica_en/3459/subview.do) for supporting this work.

