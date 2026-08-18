# Suricata

Detect HTTP communications with malicious domains identified during analysis.


```suricata
alert http any any -> any any (
    msg:"Malicious domain devbyjr.com";
    flow:established,to_server;
    http.host;
    content:"devbyjr.com";
    sid:1000001;
    rev:1;
)

alert http any any -> any any (
    msg:"Malicious domain boloshortolandia.com";
    flow:established,to_server;
    http.host;
    content:"boloshortolandia.com";
    sid:1000002;
    rev:1;
)

alert http any any -> any any (
    msg:"Malicious domain tybalties.website";
    flow:established,to_server;
    http.host;
    content:"tybalties.website";
    sid:1000003;
    rev:1;
)

alert http any any -> any any (
	msg:"Malicious domain ncvascular.com.au";
	flow:established,to_server;
	http.host;
	content:"ncvascular.com.au";
	sid:1000004;
	rev:1;
)

alert http any any -> any any (
	msg:"Malicious domain inmayjose.es";
	flow:established,to_server;
	http.host;
	content:"inmayjose.es";
	sid:1000005;
	rev:1;
)

alert http any any -> any any (
	msg:"Malicious domain lalievre.ca";
	flow:established,to_server;
	http.host;
	content:"lalievre.ca";
	sid:1000006;
	rev:1;
)

alert http any any -> any any (
	msg:"Malicious domain makmedia.ch";
	flow:established,to_server;
	http.host;
	content:"makmedia.ch";
	sid:1000007;
	rev:1;
)
```

