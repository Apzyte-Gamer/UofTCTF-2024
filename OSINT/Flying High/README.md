Flying High
=

I'm trying to find a flight I took back in 2012. I forgot the airport and the plane, but I know it is the one with an orange/red logo on the right side of this photo I took. Can you help me identify it?

The flag format is `UofTCTF{AIRPORT_AIRLINE_AIRCRAFT}`. AIRPORT is the 3 letter IATA code, `AIRLINE` is the name of the airline (dash-separated if required), and `AIRCRAFT` is the aircraft model and variant (omit manufacturer name). For example, `UofTCTF{YYZ_Air-Canada_A320-200}` or `UofTCTF{YYZ_Delta_767-300}`.

Note: The aircraft variant should be of X00 format; ie. there may be models with `XYZ-432`, but the accepted variant will be `XYZ-400`.

Author: windex

[airplane.png](./airplane.png)

Solution
=

After I saw the image, I quickly knew the aircraft was an A340 (because of its identifying features). I then looked at the `B` written on the right-most aircraft, and after a bit of searching, the airline was Iberia Airlines. Finally to find out the airport, I went on google image search and put the image. First, I saw Chalais Airport, but it wasn't the case. So I searched more until I found out it was Bordeaux Airport. I then searched up it's IATA code and BOD it was.

I then quickly put up the information and I got the flag!

`UofTCTF{BOD_Iberia-Airlines_A340}`
