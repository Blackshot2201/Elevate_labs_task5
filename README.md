# Elevate_labs_task5
# 📡 Task 5: Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective

To use Wireshark to capture live network traffic, filter by protocol, identify and analyze packets (DNS, HTTP, ICMP, TCP), and save the capture as a `.pcapng` file.

---

## 🛠️ Tools Used

* **Wireshark** – for packet capturing and analysis
* **Kali Linux** – OS used for the task
* **Protocols Examined**: DNS, HTTP, ICMP, TCP

---

## 📸 Screenshots Included

All important steps and protocol filters were captured with annotated screenshots for clarity.

---

## 🧪 Step-by-Step Procedure

---

### 1️⃣ Launch Wireshark

Opened Wireshark from Kali's app menu.

📷&#x20;

---

### 2️⃣ Start Packet Capture

Selected the `eth0` network interface and clicked **Start Capture**.

📷&#x20;

---

### 3️⃣ Generate Network Traffic

Performed the following to generate traffic:

* Opened websites (HTTP)
* Used terminal to `ping` a remote IP (ICMP)
* Browsed DNS-based URLs (DNS)

---

### 4️⃣ Stop Capture After \~1 Minute

Clicked the red square stop button to halt packet capture.

---

### 5️⃣ Filter by DNS Protocol

Used the display filter:

```wireshark
dns
```

### 6️⃣ Filter by HTTP Protocol

Used the display filter:

```
http
```

**Observation**: Captured HTTP GET requests and `200 OK` responses showing successful web page access.

---

### 7️⃣ Filter by ICMP Protocol

Used the display filter:

```
icmp
```

**Observation**: ICMP packets with “Destination Unreachable” responses due to failed ping attempts.

---

### 8️⃣ Filter by TCP Protocol

Used the display filter:

```
tcp
```

**Observation**: TCP handshakes and data packets with SYN, ACK flags indicating standard connection flow.

---

### 9️⃣ Export Capture File

Saved the captured traffic as a `.pcapng` file named:

📄 `Wireshark_capture_task5.pcapng`

---

## 🧠 What I Learned

* How to use Wireshark to analyze live traffic
* How to apply filters like `dns`, `http`, `icmp`, and `tcp`
* The role of each protocol in real network communication
* How to capture, stop, and export packet data for forensic use

---

## 📁 Files Included

```
.├── Wireshark_capture_task5.pcapng
  ├── README.md 
  ├── Dns Filter.png 
  ├── http filter.png 
  ├── icmp filter.png 
  ├── tcp filter.png 
  ├── Start capture.png 
  ├── Wireshark in kali.png
```
