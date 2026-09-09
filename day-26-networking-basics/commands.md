# Day 26 Commands — Networking Basics

1. **ip a** — Shows all network interfaces on the system along with
   their assigned IP addresses, replacing the older ifconfig command on
   most modern Linux systems.

2. **ip route** — Displays the system's routing table, including the
   default gateway — the device traffic goes through when heading
   outside the local network.

3. **ping -c** — Sends ICMP echo requests to a target host to test
   connectivity. The -c flag limits it to a specific number of pings
   instead of running indefinitely.

4. **curl** — Fetches the full content of a URL and prints it to the
   terminal, useful for testing APIs or checking what a server actually
   returns.

5. **curl -I** — Fetches only the response headers from a URL, without
   downloading the full page body — a fast way to check if a site is up
   and see server details.

6. **wget** — Downloads a file or webpage from a URL and saves it to
   disk, unlike curl which prints to the terminal by default.

7. **netstat -tulnp** — Lists listening ports along with the process
   using each one. Considered a legacy tool on many systems, replaced
   by ss, but still widely used.

8. **ss -tulnp** — The modern replacement for netstat -tulnp, showing
   listening TCP/UDP ports and the processes bound to them, generally
   faster and more detailed.

9. **hostname** — Prints the system's current hostname — the name used
   to identify the machine on a network.

10. **hostnamectl** — Shows and can set detailed system identity
    information, including hostname, OS, kernel version, and
    architecture, going beyond what hostname alone provides.
