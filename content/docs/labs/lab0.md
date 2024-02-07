---
title: Lab 0 — Introduction to Arduino
next: lab1
---

{{< callout type="error" >}}
  Note, like reading 1, this lab is designed to be sort of a "crash course" and focuses more on linking to external resources and tutorials that you might find helpful in getting familiar with Arduino. We've structured it in an order that we think helps with learning, and we are always here to offer support so please reach out if you need help!
{{< /callout >}}

Hello and welcome to class and to Lab 0! This lab is **optional to be completed on your own time** but we ask you to skim it to make sure you're comfortable with everything presented in this tutorial! We won't necessarily assumer you're perfectly familiar with everything in here, but details in Lab 0 will not be the focus of teaching for this class. It's designed to bring you up to speed. But as always, we're here to help so let us know anytime you need it! 

<div class="mt-12"></div>

{{< cards >}}
  {{< hextra/feature-card
    title="Basic Arduino Getting Started"
    subtitle="A general overview of the Arduino platform."
    link="https://docs.arduino.cc/learn/starting-guide/getting-started-arduino/"
  >}}
  {{< hextra/feature-card
    title="Arduino IDE"
    subtitle="Overview of the desktop programming environment, note this also contains a small version of the Blink tutorial."
    link="https://docs.arduino.cc/learn/starting-guide/the-arduino-software-ide/"
  >}}
{{< /cards >}}

## The Classic Arduino Blink Tutorial

Blink is a basic tutorial with Arduino that lets you connect an LED to the board and make it flash at a specified frequency. Note that you can do this with an external LED, but all arduinos have an in-built LED as well. We haven't given you external LEDs or resistors, so try to make this tutorial work with the built in LED. **Note the tutorials in the previous section can help you in getting the Arduino connected to the programming environment.**

{{< cards >}}
  {{< hextra/feature-card
    title="Arduino Blink Tutorial"
    subtitle="Connect the Arduino to the computer and make the LED flash!"
    link="https://docs.arduino.cc/built-in-examples/basics/Blink/"
  >}}
{{< /cards >}}

The Blink tutorial is great because it gets you started with Arduino, familiar with the board and the programming environment, and it's a great way to check that your Arduino works with a visual indication. Sometimes in embedded systems, it's difficult because we can't "see" the code running on the microcontroller.

## Hello World but with Arduino

Hello World is a classic tutorial for all programming languages. Here we're going to get the Arduino to print "Hello World" to what's called the serial terminal. 

{{< cards >}}
  {{< hextra/feature-card
    title="Hello World w/ Arduino"
    subtitle="Introduction to using the Arduino Serial Monitor and printing information to the terminal."
    link="https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-serial-monitor/"
  >}}
  {{< hextra/feature-card
    title="Printing Variables"
    subtitle="Note that you can also print the value of a variable in many formats!"
    link="https://www.arduino.cc/reference/en/language/functions/communication/serial/println/"
  >}}
{{< /cards >}}

### Information on Serial Communications

Serial Communications is a class of communications protocols that send bits of data over a digital interface one after another (hence serial). Arduino uses UART which is Universal Asynchronous Recieve and Transmit, and this is how the computer communicates with your Arduino when its plugged in over USB.

{{< cards >}}
  {{< hextra/feature-card
    title="UART"
    subtitle="Basic information about UART from our friends at Analog Devices."
    link="https://www.analog.com/en/resources/analog-dialogue/articles/uart-a-hardware-communication-protocol.html"
  >}}
{{< /cards >}}

## Controlling a Servo with Arduino

A servo motor is a small motor with an internal position controller. The arduino can send signals to control the position of the motor. For example, if we wanted to open and close a small door in an automatic food dispenser for a cat, we could use a servo.

{{< cards >}}
  {{< hextra/feature-card
    title="Servo Control with Arduino"
    subtitle="Tutorial on connecting a small servo to arduino and making it move."
    link="https://docs.arduino.cc/tutorials/generic/basic-servo-control/"
  >}}
{{< /cards >}}

## Basic Logic Tutorials

Now that we've moved a servo and controlled an LED, we can think about more complex logic systems including using buttons to activate actions. The most basic way to do this is an if-then statement.

{{< cards >}}
  {{< hextra/feature-card
    title="Button and LED with Arduino"
    subtitle="How to make a button turn an LED on and off with Arduino."
    link="https://docs.arduino.cc/built-in-examples/digital/Button/"
  >}}
{{< /cards >}}

## Functions in Arduino

Functions are a basic programming technique used when we want to clean up a code file or when a code snippet will be repeatedly used often. It's also often used when we want to pass data to a set of code for processing. You can read more about functions and learn to use them in the below tutorial.

{{< cards >}}
  {{< hextra/feature-card
    title="Functions in Arduino"
    subtitle="Help yourself write cleaner code by learning about functions!"
    link="https://docs.arduino.cc/learn/programming/functions/"
  >}}
{{< /cards >}}

*Note, the last part of the tutorial reads from an analog sensor. We haven't taught you to do that yet, so don't worry if it doesn't make sense!*

## Challenge

Here's a challenge to try on your own! Did you know you can give inputs to the Arduino from the serial monitor? Check out [this tutorial video on YouTube ↗](https://www.youtube.com/watch?v=XishaRwUlGM). See if you can write a calculator that takes two numbers as an input, multiplies them together, and displays the result in the serial monitor!

## Variables, Datatypes, Constants

In programs, we use variables and data structures to store data. Here we present some resources to learn about variables and data types.

{{< cards >}}
  {{< hextra/feature-card
    title="Using Variables in Arduino"
    subtitle="Here's a basic tutorial on variables and the scope of variables."
    link="https://docs.arduino.cc/learn/programming/variables/"
  >}}
{{< /cards >}}

Now different types of variables exist, they can store different things, and they use different amounts of memory to do that. These are called data types. We can also define constants in Arduino. It's not necessary to understand these in great great detail, but it's important to think about when you would use what kind of variable.

{{< cards >}}
  {{< hextra/feature-card
    title="List of all Arduino Data Types"
    subtitle="Here you find documentation on all the arduino variable types and how to use them."
    link="https://www.arduino.cc/reference/en/#variables"
  >}}
  {{< hextra/feature-card
    title="Constants in Arduino"
    subtitle="Constants cannot be changed without re-uploading the program. But they're very useful in defining things like pin numbers and more!"
    link="https://www.arduino.cc/reference/en/language/variables/variable-scope-qualifiers/const/"
  >}}
{{< /cards >}}

Sparkfun has a [great tutorial on data types and why you might want to use certain types ↗](https://learn.sparkfun.com/tutorials/data-types-in-arduino/all).

## Fun Arduino Projects to Inspire You!

There's lots of things you can connect to an arduino to make super awesome things! Here's a few just to get you thinking! We'll cover many more in the class itself.

{{< cards >}}
  {{< hextra/feature-card
    title="Save the Elephants!"
    subtitle="Mahout is an organization focused on conservation of Asian elephants. They put collars on the elephants to help track them and also understand their behvaioral patterns! This is one of my favorite Arduino projects."
    link="https://www.hackster.io/mithun-das/mahout-save-the-elephants-819b54"
  >}}
  {{< hextra/feature-card
    title="Irrigation, and Crop Monitoring"
    subtitle="Challenge agriculture uses tensiometry to measure the water content of soil for smart irrigation. They do multi-level imaging of the soil, for irrigation monitoring, prevention of soil degradation and road cracking, and even more!"
    link="https://www.challenge-agriculture.fr/en/tensiometry/what-is-tensiometry/"
  >}}
  {{< hextra/feature-card
    title="Arduino at the Edge of Space!"
    subtitle="Here's a super fun project, buidling an Arduino weather balloon with a datalogger! Weather balloons are super cool because they allow scientists to study weather at atmospheric patterns."
    link="https://projecthub.arduino.cc/nmrsthrust/arduino-powered-weather-balloon-datalogger-e88691"
  >}}
  {{< hextra/feature-card
    title="Medical Devices"
    subtitle="MySignals is an IoT development platform for medical devices powered by Arduino. It has a number of sensors such as SPO2, Temperature, EMG, ECG, Blood Pressure and more. And has the ability to add custom sensors all streamed to an online platform. Likely not avaliable anymore to data privacy concerns, it is an example of how Arduino could make medical devices more accessible."
    link="https://www.youtube.com/watch?v=MiMDOT-Wt4w"
  >}}
{{< /cards >}}

Here is some [more info on Tensiometry ↗](https://sanangelo.tamu.edu/extension/agronomy/agronomy-publications/grain-sorghum-production-in-west-central-texas/how-to-estimate-soil-moisture-by-feel/soil-moisture-measuring-devices/tensiometer/#:~:text=In%20essence%2C%20the%20tensiometer%20gauges,on%20the%20tensiometer%20vacuum%20gauge.) if you're interested! 




