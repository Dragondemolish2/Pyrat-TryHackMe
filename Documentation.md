Step 1 is always scan the target to identify any open ports to start looking into the target.

<img width="943" height="780" alt="Screenshot 2026-02-24 192431" src="https://github.com/user-attachments/assets/51f648d9-7505-4221-9862-c05972c6f779" />

After the scan we can inspect the open ports first through the most obvious way http.

<img width="946" height="783" alt="Screenshot 2026-02-24 192359" src="https://github.com/user-attachments/assets/7e94d555-72f7-4c0d-90bd-28470b3eb3e2" />

Netcat
(often abbreviated as nc) is considered a "more basic" connection tool because it interacts directly with network sockets (TCP/UDP) with minimal abstraction, overhead, or built-in protocols. It operates as a raw "pipe" that simply sends and receives data, making it a foundational tool for debugging, data transfer, and port manipulation

So we use nc to connect to the http server.

<img width="600" height="54" alt="Screenshot 2026-02-24 192530" src="https://github.com/user-attachments/assets/f940ce3e-81ba-41f6-a47e-7f951e225703" />

When then notice the normal linux commands dont work and try some python commands which does work and as hinted at in the question we also try to setup a reverse shell to access the rest of the server.

<img width="919" height="795" alt="Screenshot 2026-02-24 192509" src="https://github.com/user-attachments/assets/421c26c4-b1a1-47d4-b036-1c87003ed340" />

<img width="652" height="430" alt="Screenshot 2026-02-24 192705" src="https://github.com/user-attachments/assets/b5b0b005-e633-4938-9f74-f2eb44c62046" />

We then also listen to the port we specified tp access the reverse shell.

<img width="859" height="622" alt="Screenshot 2026-02-24 192730" src="https://github.com/user-attachments/assets/2b6d81c8-5869-4c4b-b024-7e6130f9ca9b" />

