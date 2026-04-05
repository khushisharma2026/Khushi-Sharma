### **Overview**
#### Ariane 5 Flight 501 – Quick Facts
| Ariane 5 Flight 501 | |
|---------------------|--|
| Date                | June 4, 1996 |
| Agency              | ESA |
| Outcome             | Failure (37 seconds after launch) |
| Cause               | Software error (overflow) |
| Loss                | ~$370 million |

The Ariane 5 was developed by the [European Space Agency](https://en.wikipedia.org/wiki/European_Space_Agency) as part of a long-term effort to maintain Europe's access to space. In the 1985 Ministeral Conference, ESA decided to create a more powerful launch vehicle than Ariane 4 and to supporrt future missions, including taking part in space stations proposed by [NASA](https://en.wikipedia.org/wiki/NASA). The Ariane 5 was officialy aprroved at the 1987 Ministeral Conference. It was designed to carry heavy payloads into Low-Earth Orbit, Geostationary Orbit and Sun-synchronous Orbit.

The first launch, known as [Ariane 5 Flight 501](https://en.wikipedia.org/wiki/Ariane_flight_V88), took place on June 4, 1996. The launch ended in failure just 37 seconds after the liftoff. Shortly after the launch, the rocjet deviated from its intended trajectory and disintegrated. The second test flight (502) on  30th October 1997 was a partial failure. The third test flight (503) on 21st October 1998 was a success.

As a safety measure, the onboard self-destruct system was activated, resulting in the complete loss of the vehicle and its payload. 
The nature of the failure was related to the rocket's guidance and control system. The failure was not caused by any mechanical or structural defect, but by incorrect data being sent to the onboard computer. This led the rocket to make sudden and unnecessary adjustments in its flight path, which ultimately caused it to break apart.
The root cause of the failure was a software error in the Inertial Reference System (IRS). This was responsible for aligning the rockets before take-off. It was used to check if the velocity of the rocket is increasing or decreasing, and this is known as horizontal bias or BH value.
 The issue occured because software from Ariane 4 was reused without fully adapting it to the different flight conditions of Ariane 5. Specifically, the system attempted to convert a 64-bit floating-point number into a 16-bit signed integer.
During the early phase of the flight, this conversion worked correctly because the rocket's velocity remained within acceptable limits. However, as the rocket accelerated, the value exceeded the maximum limit of the 16-bit integer, resulting in an overflow error. Instead of handling this error safely, the system shut down and produced a diagnostic value that was intended only for debugging purposes.

The consequences of the failure were significant. The rocket and its payload were completely destroyed, resulting in an estimated financial loss around $370 million. In addition to the economic impact, the failure damaged the reputation of ESA and delayed the Ariane 5 programme. However, it also led to important improvements in software testing, validation, and safety practices in aerospace engineering.

In conclusion, the Ariane 5 Flight 501 failure was primarily a software and design failure rather than a hardware issue. While the immediate cause was a software bug, the deeper problwm was the decision to reuse outdated code without proper modification and the lack of adequate error handling. this case remains one of the most well-known examples of how small software errors  can lead to damaging consequences in complex engineering systems.

SUMMARY OF THE BOOK
**_Fail Better: The science of Right Kind of Wrong_**

* There are four key attributes that make a failure an intelligent failure:
  * 1. the failure takes place in a new territory,
    * 2. the failure is made towards a desired and meaningful goal ,
  *  3.it is informed by available knowledge and
  * 4.the failure is as small as it can still provide valuable insights.

