# Robot Builders Night Virtual for July 14th, 2026

## [RBNV 2026 July 14/2026 - YouTube](https://www.youtube.com/watch?v=aSJUYdMdf9w)

## Main Discussion Points

**Autonomous RC Car** - Yahya shared progress on an obstacle-avoiding RC car. The group jumped in to help troubleshoot communication issues between the Arduino, steering servo, and Electronic Speed Controller (ESC). Suggestions included verifying PWM pins, focusing on the steering servo first, and utilizing affordable diagnostic tools like servo testers and $10 logic analyzers. Mark D. also offered in-person debugging help at the Dallas Makerspace.

**Vintage RC Transmitter Conversion** - Tom C. showed off a fantastic side project converting a high-quality, 1970s-era radio transmitter enclosure to control a modern outdoor robot. He replaced the old electronics with an ESP8266, custom voltage regulators, and an analog multiplexer to handle the joysticks and switches.
LoRa Remote Control: Ray C. demonstrated his long-range LoRa controller featuring a built-in OLED display, designed as an effective dead-man switch for heavy autonomous mowers.

**Autonomous Mower & Robbie Update** - Paul B. celebrated a milestone with his mower successfully navigating one meter autonomously using RTK GPS. Gold star ⭐

- He also gave an update on the "Roby" robot project for Moon Day; the team has successfully implemented face tracking using MediaPipe, but is currently troubleshooting a webcam color distortion issue that broke the face recognition.

**AI in Engineering Workflows** - Chris N. presented how he successfully leveraged high-end AI models (Fable 5 and GPT 5.6 Soul) to fix a complex LiDAR distortion algorithm that was warping mapping data during robot rotation.  Black star ★

- This led to a group-wide philosophical discussion on managing AI workflows. Harold P., Carl O., and Chris N. discussed the importance of defining constraints, feeding AI proper contexts, and budget-saving strategies—such as using high-end models to draft strategic plans and cheaper models to write the actual code.  The group touched on using AI "deep research" modes for accurate, cited research. Chris N. emphasized that the real future of scaling AI in robotics is "closing the loop" creating infrastructure where the AI can automatically test its own code on target embedded hardware and fix its own errors.
  Tech Highlights - Chris N. shared an uneventful but fascinating anecdotal experience riding in a Waymo robotaxi in San Francisco.

**Paul B**. presented a video of advanced 1x robot hands featuring 32 degrees of freedom, tendon-based operation, and force feedback capabilities capable of 45 Newtons (about 10 pounds) of force per finger.

## Conclusions and Insights

- Participants exchanged practical advice on robotics tools, with useful links for purchasing and understanding technical specifications.
- Technical discussions included converting force measurements to better understand the specs and capabilities of robotics equipment.

## Referenced Links

### Provided by Pat Caron

- [DKARDU Logic Analyzer for Arduino](https://www.amazon.com/DKARDU-Analyzer-Device-Channel-Arduino/dp/B09BPV5QNQ/ref=sr_1_3_sspa)

### Provided by Carl Ott

- [DIYmall Consistency Controller Servo Tester](https://www.amazon.com/DIYmall-Consistency-Controller-Helicopter-Airplane/dp/B07FQNZHG4)

### Provided by Tom Crawford

- [AliExpress Servo Tester](https://www.aliexpress.com/item/1005005249039826.html?src=bing&exp_tag=pcgcp&albch=shopping&acnt=135095331&albcp=412811419&albag=1311717734383599&slnk=&trgt=pla-4585581970548950&plac=&crea=81982433154568&netw=s&device=c&mtctp=e&utm_source=Bing&utm_medium=shopping&utm_campaign=PA_Bing_CA_PLA_customlabel7_TROAS_AESupply_24.6.3&utm_content=customlable1%3D7&utm_term=aliexpress+servo+tester&msclkid=084b564dea531a2496df3c1b36f82307&aff_fcid=b742ea3c0ea1426f8eb6b367cdb2e428-1784077489026-05181-UneMJZVf&aff_fsk=UneMJZVf&aff_platform=aaf&sk=UneMJZVf&aff_trace_key=b742ea3c0ea1426f8eb6b367cdb2e428-1784077489026-05181-UneMJZVf&terminal_id=7695f25e5bc74321b2554e6daa2146e3&afSmartRedirect=n)
- [Using Your Computer’s Sound Card as a Scope](https://www.nutsvolts.com/magazine/article/turn-your-computers-sound-card-into-a-scope)

### Provided by Paul Bouchier

- [Neos Hands Robotics](https://www.1x.tech/discover/neos-hands)