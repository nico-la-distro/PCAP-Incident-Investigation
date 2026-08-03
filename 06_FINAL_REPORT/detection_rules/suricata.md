**Objective:** 

Detect HTTP communications with malicious domains identified during PCAP analysis.


```suricata
alert http any any -> any any (
    msg:"PCAP Investigation - Malicious domain devbyjr.com";
    flow:established,to_server;
    http.host;
    content:"devbyjr.com";
    sid:1000001;
    rev:1;
)

alert http any any -> any any (
    msg:"PCAP Investigation - Malicious domain boloshortolandia.com";
    flow:established,to_server;
    http.host;
    content:"boloshortolandia.com";
    sid:1000002;
    rev:1;
)

alert http any any -> any any (
    msg:"PCAP Investigation - Malicious domain tybalties.website";
    flow:established,to_server;
    http.host;
    content:"tybalties.website";
    sid:1000003;
    rev:1;
)
```

