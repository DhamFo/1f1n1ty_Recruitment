Basic SSRF against another back-end system:

    -The application server is able to interact with back-end systems that are not directly reachable by users. These systems often have non-routable private IP addresses
    -The back-end systems are normally protected by the network topology.Internal back-end systems contain sensitive functionality that can be accessed without authentication by anyone who is able to interact with the systems
    -stockApi=http://192.168.0.x:8080/admin we use intruder to search from 1 to 255 in burp suite.
    -If the reesponse is 200 then we need to chk that particular adress for the lab