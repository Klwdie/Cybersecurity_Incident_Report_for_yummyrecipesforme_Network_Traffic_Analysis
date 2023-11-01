# Cybersecurity Incident Report for Yummy Recipes For Me: Network Traffic Analysis

---

While working as a security analyst at a (**fictional**) company that specializes in providing IT consultant services, customers contacted our company to report that they were unable to access the company website **www.yummyrecipesforme.com**, and saw the error “**destination port unreachable**” after waiting for the page to load. 

I was then tasked with analyzing the situation and determining which network protocol was affected during this incident. I began by visiting the website where I also received the error “**destination port unreachable**”. Next, I loaded my network analyzer tool, **tcpdump**, and refreshed the webpage. This time, I captured packets to review using **tcpdump**. The resulting logs reveal that when UDP packets were sent and received an ICMP response, returned to my host, the results contained an error message: “**udp port 53 unreachable**”.

*The tcpdump logs can be found in this repository.*

After analyzing the data packets captured using **tcpdump**, I have identified which network protocol and service were impacted by this incident and have written a follow-up report. *This follow-up report can be found in this repository.* This incident, in the meantime, is being handled by security engineers after I and other analysts have reported the issue to our direct supervisor. 

---
