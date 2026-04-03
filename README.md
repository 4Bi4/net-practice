*This project has been created as part of the 42 curriculum by labia-fe.*

# NetPractice

## Description

NetPractice is a practical networking exercise from the 42 curriculum. The goal is to configure small-scale simulated networks by solving 10 progressive levels, each presenting a broken network diagram that must be fixed by adjusting IP addresses, subnet masks, and routing configurations.

Through this project, you will gain hands-on experience with the fundamentals of TCP/IP networking — understanding how devices communicate, how traffic is routed between networks, and how to correctly assign addresses so that every host can reach its destination.

---

## Instructions

### Running the Training Interface

1. Download the project files from the project page.
2. Extract them into a folder of your choice.
3. In that folder, run the launch script:

```bash
bash run.sh
```

This will start a local web server and open the NetPractice interface in your browser.

> **If `run.sh` doesn't work**, start the server manually:
> ```bash
> python3 -m http.server 49242
> ```
> Then open your browser and navigate to `http://localhost:49242`.

### Using the Interface

- On the login screen, enter your **42 intranet login** in the field provided — this generates your personal configuration.
- Use the **Training** tab to practice your levels.
- Use the **Evaluation** tab to generate a random configuration (also valid for defense).

### Completing and Exporting Levels

- For each level, a non-functioning network diagram is displayed.
- Modify the **unshaded fields** (IP addresses, masks, routes) until the network works correctly.
- Click **[Check again]** to validate your configuration.
- Once a level is solved, click **[Get my config]** to download your configuration file.
- Click **[Next level]** to proceed.

> ⚠️ Do **not** forget to export your config before moving to the next level — you cannot go back.

### Submission Requirements

- Complete all **10 levels**.
- Place the **10 exported configuration files** (one per level) at the **root of your Git repository**.
- Make sure your **login was entered** in the interface before exporting — it is embedded in the config files and used during evaluation.

---

## Resources

### Networking Concepts Studied

- **TCP/IP Addressing** — how IP addresses identify devices on a network
- **Subnet Masks** — how masks define the network and host portions of an address
- **CIDR Notation** — shorthand for expressing subnet masks (e.g., `/24`)
- **Default Gateways** — the router interface a host uses to reach outside its subnet
- **Routing Tables** — how routers decide where to forward packets
- **Routers and Switches** — their roles and differences in a network topology
- **OSI Model Layers** — conceptual framework for understanding network communication

### References

- [Cisco Networking Basics](https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/networking-basics.html)
- [Subnet Mask Cheat Sheet](https://www.aelius.com/njh/subnet_sheet.html)
- [IP Addressing and Subnetting Guide — Cisco](https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html)
- [What is a Default Gateway? — Cloudflare](https://www.cloudflare.com/learning/network-layer/what-is-a-router/)
- [OSI Model Explained — Cloudflare](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
- [ipcalc — IP Calculator](https://jodies.de/ipcalc)

### AI Usage

AI (Claude) was used during this project for the following tasks:

- **Concept clarification**: asking for plain-language explanations of subnetting, CIDR, and routing table logic when documentation was unclear.
- **Debugging help**: describing a misconfigured network state and asking what might be wrong to guide my own investigation.
- **README drafting**: generating a first draft of this file, which was then reviewed and adapted.

All AI-generated content was reviewed, tested, and validated personally before use.
