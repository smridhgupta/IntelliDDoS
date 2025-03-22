# IntelliDDoS - AI-based DDoS Framework

IntelliDDoS is an advanced AI-based framework for simulating and executing Distributed Denial of Service (DDoS) attacks. This powerful tool utilizes neural networks and reinforcement learning techniques to dynamically optimize attack strategies, making it one of the most robust and effective DDoS simulation frameworks available.

## Features

- **Multiple Attack Modes**: Supports flood, hold, and WebSocket attack modes.
- **Dynamic Mode Switching**: Automatically switches attack modes based on target server's response.
- **AI and Machine Learning**: Utilizes reinforcement learning to optimize attack parameters.
- **Scalable**: Adjusts resources based on system capabilities.
- **Cross-Platform**: Compatible with macOS, Linux, and Windows.
- **High Performance**: Capable of generating a high volume of requests and maintaining persistent connections to test server resilience.
- **Detailed Monitoring**: Provides real-time updates on attack status, including successful and failed requests, errors, and connection resets.

## Power and Capability

### High Request Volume
IntelliDDoS can generate a massive number of requests per second, overwhelming even the most robust servers. Its flood mode is designed to test the upper limits of server capacity.

### Persistent Connections
The hold mode opens and maintains persistent connections, exhausting server resources over time. This is particularly effective against servers with connection limitations.

### Advanced WebSocket Attacks
The WebSocket mode takes advantage of WebSocket connections to perform sophisticated attacks, capable of bypassing traditional security measures that may block HTTP-based DDoS attempts.

### Intelligent Adaptation
Using AI and machine learning, IntelliDDoS continually learns and adapts its attack strategies based on server responses. This ensures that the attack remains effective even as the server attempts to mitigate the impact.

### Resource Optimization
IntelliDDoS automatically adjusts its resource usage based on the capabilities of the host system, ensuring optimal performance without overwhelming the attacker's hardware.

### Real-Time Analysis
The framework provides real-time analysis of the attack's effectiveness, allowing users to monitor success rates, error rates, and other critical metrics. This feedback loop ensures that the attack remains potent throughout its duration.

## Comparison with Other Frameworks

When comparing IntelliDDoS to well-known DDoS frameworks or tools (like LOIC, HOIC, Slowloris), several aspects are noteworthy:

### Complexity and Sophistication

- **IntelliDDoS**: Uses advanced techniques such as machine learning and asynchronous programming to adapt and potentially optimize the attack strategies based on real-time feedback.
- **Traditional Tools**: Tools like LOIC or HOIC are typically more straightforward, with predefined attack patterns and less adaptability. They focus on overwhelming a target through volume rather than adapting tactics based on server response.

### Flexibility and Scalability

- **IntelliDDoS**: Highly scalable due to its asynchronous design and can adjust its attack pattern dynamically. It is designed to evade detection by altering its behavior (like changing user agents, IPs, generates ssl context, xml data, random data, json data, random cookies, headers and form data, has random delays etc.).
- **Traditional Tools**: Often lack scalability or the ability to change tactics mid-attack, making them more predictable and easier to mitigate.

### Effectiveness

- **IntelliDDoS**: Potentially more effective due to its adaptive nature, though its real-world effectiveness would depend significantly on how well the machine learning model is trained and the environment in which it's deployed.
- **Traditional Tools**: Effectiveness can be high for specific targets but generally lacks adaptability to changing defenses or network conditions.

### Detection and Mitigation

- **IntelliDDoS**: Might be harder to detect initially due to its adaptive tactics. However, sophisticated network monitoring tools and defensive strategies can still mitigate its impact.
- **Traditional Tools**: Easier to detect due to predictable patterns and commonly known signatures.

## Prerequisites

Ensure you have the following installed:

- Python 3.11
- Required Python libraries:
  ```sh
  pip3 install aiohttp websockets numpy psutil tensorflow scikit-learn pycryptodome
  ```

## Setup

1. **Clone the repository**:
   ```sh
   git clone https://github.com/smridhgupta/IntelliDDoS.git
   cd IntelliDDoS
   ```

## Usage

1. **Start the script**:
   ```sh
   python3.11 IntelliDDoS.py
   ```

2. **Enter the target URL**:
   When prompted, enter the target URL you wish to test.

3. **Monitor the attack**:
   The script will display the current attack status and switch modes automatically based on the server's response.

## Modes

- **Flood Mode**: Sends a high volume of requests to overwhelm the server.
- **Hold Mode**: Opens and holds connections for an extended period using different techniques.
- **WebSocket Mode**: Utilizes WebSocket connections for the attack.

## Performance Evaluation

The framework evaluates performance based on success rates, error rates, and connection reset errors. It dynamically adjusts attack parameters using a Q-learning-based reinforcement learning algorithm.

## Donate

. BTC: bc1qykzfyjdkyck5v4sd46j4y8ra6mgltvu6zqu69s

## Disclaimer

This tool is intended for educational and research purposes only. The author is not responsible for any misuse of this tool. Use it responsibly and only on servers you own or have permission to test.

The developer retains the copyright to the script uploaded on this repository. This script is provided for educational and informational purposes only.

The developer makes no representations or warranties regarding the accuracy or completeness of the script. Users downloading or utilizing the script do so at their own risk and discretion. The developer shall not be liable for any direct, indirect, incidental, special, or consequential damages arising out of the use or inability to use the script.

By downloading or using the script, you agree to abide by the terms and conditions mentioned here. If you have any questions or need further information, please contact the developer Smridh Gupta, Email- smridhgupta@proton.me.

## Contribution

Contributions are welcome! Please submit a pull request or open an issue for any enhancements or bug fixes.

## Contact

For any queries or support, contact smridhgupta@proton.me

Developed by @smridhgupta

---

**Note**: The actual implementation details and sensitive parts of the code are obfuscated for copyright and security reasons.
