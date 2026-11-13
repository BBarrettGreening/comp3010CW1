# COMP3010 CW1 – Evidence Portfolio

Evidence for the CW1 intrusion investigation of `COMP3010CW1.pcap`

## AI use logs

AI was used as a partner throughout, through the open-weights model **qwen3:14b**, running locally with Ollama and the `pi` client. Every command was run by hand, and its output was pasted into the chat.

| File | Date | Contents |
|---|---|---|
| `system_prompt.md` | – | Role and rules given to the model: no invented values, a command behind every claim, UTC timestamps, no internet search without permission |
| `mac_address_session.html` | 23 Oct 2026 | Interpreting tshark endpoint and conversation output to identify the infected host's MAC and IP addresses |
| `hostname_session.html` | 23 Oct 2026 | Finding the hostname. The model invented an IP address and gave DHCP field names that tshark rejected. The working DHCP option 12 filter came from the tshark documentation |
| `infection_date_session.html` | 23 Oct 2026 | Approach for dating the infection. Source of the tcpdump host filter and the tshark time export used for the timeline |
| `report_session.html` | 11 Nov 2026 | Report planning. The findings and section plan were provided, with an instruction not to write the report. The model suggested evidence, styling and a word budget per section |

The `.html` files are self-contained exports of each `pi` session. Open them in a browser to read the full conversation.
