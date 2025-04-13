# 📡 TShark: Terminal-Based Wireshark

TShark is the command-line interface (CLI) version of Wireshark, designed for capturing and analyzing network traffic without the need for a graphical user interface. It's ideal for remote diagnostics, automation, and environments where GUI tools are unavailable.

---

## 🔧 Key Features

- **Live Packet Capture**: Capture network traffic in real-time from specified interfaces.
- **File Analysis**: Read and analyze packets from existing capture files.
- **Filtering**: Apply capture and display filters to isolate specific traffic.
- **Protocol Dissection**: Supports detailed analysis of numerous protocols.
- **Output Flexibility**: Display summaries or detailed packet information; export to various formats.
- **Automation-Friendly**: Suitable for scripting and integration into automated workflows.

---

## 🛠️ Common Command-Line Options

### Capture Options

- `-i <interface>`: Specify the capture interface (e.g., `eth0`).
- `-f "<filter>"`: Apply a capture filter using libpcap syntax (e.g., `tcp port 80`).
- `-s <snaplen>`: Set the snapshot length for captured packets.
- `-p`: Disable promiscuous mode.
- `-B <buffer size>`: Set the kernel buffer size in MiB.
- `-D`: List available interfaces.

### Output Options

- `-w <file>`: Write captured packets to a file.
- `-c <count>`: Stop capture after a specified number of packets.
- `-a <condition>`: Set autostop conditions (e.g., duration, filesize).
- `-b <ringbuffer options>`: Enable ring buffer with specified parameters.

### Display and Processing

- `-V`: Display packet details.
- `-O <protocols>`: Show details for specified protocols.
- `-n`: Disable name resolution.
- `-Y "<display filter>"`: Apply a display filter using Wireshark syntax.
- `-r <file>`: Read packets from a capture file.

---

## 🧪 Example Commands

- **Capture HTTP Traffic on Interface eth0**:
  ```bash
  tshark -i eth0 -f "tcp port 80"
  ```

- **Read and Display Packets from a File**:
  ```bash
  tshark -r capture.pcap
  ```

- **Capture and Save to File with a Display Filter**:
  ```bash
  tshark -i eth0 -Y "http.request" -w http_requests.pcap
  ```

- **List Available Interfaces**:
  ```bash
  tshark -D
  ```

---

## 📚 Additional Resources

- [TShark User's Guide](https://www.wireshark.org/docs/wsug_html_chunked/AppToolstshark.html)
- [TShark Man Page](https://www.wireshark.org/docs/man-pages/tshark.html)
- [Wireshark Display Filter Reference](https://www.wireshark.org/docs/dfref/)

---

*Note: Ensure you have the necessary permissions to capture packets on your system. Running TShark may require elevated privileges.*
