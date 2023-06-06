# Performance-Testing-Booking-API

## How to run this project
- Clone this project
- Open with JMeter / Command Shell
- Run Command:
```bash
jmeter -n -t Hotel_Booking_T100.jmx -l report\Hotel_Booking_T100.jtl
jmeter -g report\Hotel_Booking_T100.jtl -o report\Hotel_Booking_T100.html

jmeter -n -t Hotel_Booking_T150.jmx -l report\Hotel_Booking_T150.jtl
jmeter -g report\Hotel_Booking_T150.jtl -o report\Hotel_Booking_T150.html

jmeter -n -t Hotel_Booking_T200.jmx -l report\Hotel_Booking_T200.jtl
jmeter -g report\Hotel_Booking_T200.jtl -o report\Hotel_Booking_T200.html

jmeter -n -t Hotel_Booking_T250.jmx -l report\Hotel_Booking_T250.jtl
jmeter -g report\Hotel_Booking_T250.jtl -o report\Hotel_Booking_T250.html
```
## Technology used:
- JMeter

## Pre-requisite:
- Jdk
- JMeter

## 🔗 API Documentation:
https://restful-booker.herokuapp.com/apidoc/index.html#api-Booking

## Reporting in jmeter

I’ve completed performance test on frequently used API for test App. 
Test executed for the below mentioned scenario in server 000.000.000.00. 

100 Concurrent Request with 10 Loop Count; Avg TPS for Total Samples is ~ 2.37 And Total Concurrent API requested: 200.
150 Concurrent Request with 10 Loop Count; Avg TPS for Total Samples is ~ 5.0 And Total Concurrent API requested: 300.
200 Concurrent Request with 10 Loop Count; Avg TPS for Total Samples is ~ 6.2 And Total Concurrent API requested: 400.
250 Concurrent Request with 10 Loop Count; Avg TPS for Total Samples is ~ 4.20 And Total Concurrent API requested: 500.

While executed 250 concurrent request, error rate is 0.00%. 

Summary: Server can handle almost concurrent 500 API call with almost zero (0) error rate.

Please find the details report from the attachment and  let me know if you have any further queries.
