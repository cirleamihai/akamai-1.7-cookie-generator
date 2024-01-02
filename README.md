# akamai-1.7-cookie-generator
<h2> disclaimer: 2021 working version -> might be outdated </h2>
<h1>Welcome to Akamai Cookie Generator for SizeerBot!</h1>
    <p>This script is designed to automate the process of generating valid Akamai cookies for interacting with websites protected by Akamai's Bot Manager, specifically targeting the Sizeer website.</p>

    <h2>What is Akamai?</h2>
    <p>Akamai Technologies is a global content delivery network (CDN), cybersecurity, and cloud service company, providing web and Internet security services. Akamai's Bot Manager is a tool that websites use to protect themselves against automated bots. It scrutinizes the traffic and distinguishes between legitimate users and bots.</p>

    <h2>Overview of SizeerBot</h2>
    <p>SizeerBot is a sophisticated bot designed to interact with the Sizeer website. It emulates human-like interactions to browse the website, add items to the cart, and check out. The script provided is a part of SizeerBot that specifically deals with generating Akamai cookies needed to bypass the bot protection on the Sizeer website.</p>

    <h2>Prerequisites</h2>
    <p>Before you start using this script, ensure you have the following:</p>
    <ul>
        <li><strong>Python Environment</strong>: A Python environment with Python 3.6 or higher installed.</li>
        <li><strong>Required Libraries</strong>: Ensure all dependencies are installed using <code>pip install -r requirements.txt</code> where <code>requirements.txt</code> includes:</li>
        <ul>
            <li>pymongo</li>
            <li>requests</li>
            <li>js2py</li>
            <li>hashlib</li>
            <li>datetime</li>
            <li>random</li>
        </ul>
        <li><strong>MongoDB Database</strong>: Access to a MongoDB database containing canvas information generally used for browser fingerprinting. Update the <code>CONNECTION_STRING</code> with your MongoDB connection string.</li>
    </ul>

    <h2>How to Use</h2>
    <h3>Step 1: Setup</h3>
    <p>Clone the repository to your local machine and navigate to the script's directory. Install the required Python libraries.</p>
    <pre>
        <code>
git clone [repository link]
cd [repository directory]
pip install -r requirements.txt
        </code>
    </pre>

    <h3>Step 2: Configure MongoDB</h3>
    <p>Ensure your MongoDB database is set up and contains the necessary canvas fingerprinting data. Update the <code>CONNECTION_STRING</code> in the script with your connection details.</p>

    <h3>Step 3: Understanding the Script</h3>
    <p>The script is divided into several classes:</p>
    <ul>
        <li><code>Abck</code>: Handles operations related to Akamai's sensor data generation.</li>
        <li><code>Akamai</code>: The main class responsible for assembling and managing the sensor data needed for cookie generation.</li>
        <li><code>SizeerBot</code>: An example bot that utilizes the <code>Akamai</code> class for generating a valid <code>_abck</code> cookie.</li>
    </ul>

    <h3>Step 4: Running the Script</h3>
    <p>Execute the script using Python.</p>
    <pre>
        <code>
python [script_name].py
        </code>
    </pre>

    <h3>Step 5: Implementing Your Bot</h3>
    <p>Use the <code>SizeerBot</code> class as a template to integrate the Akamai cookie generation into your bot. You'll need to fill in the necessary details and expand on the methods according to your bot's workflow.</p>

    <h2>Important Notes</h2>
    <ul>
        <li>This script is for educational purposes and understanding how to navigate complex web security.</li>
        <li>The effectiveness of the script can vary based on Akamai's updates and the specific configurations of the target website.</li>
        <li>Respect the website's terms of service. Using bots can be against the terms of service of many websites.</li>
    </ul>

    <h2>Conclusion</h2>
    <p>With this script, you're well on your way to understanding and navigating the complexities of web security implemented by Akamai. Remember, the key to successful botting is not just about getting past security measures but also ensuring your bot behaves responsibly and ethically. Happy coding!</p>
