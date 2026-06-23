# NTL Production Command Center

A live, web-based production tracking application designed for garment manufacturing facilities. This tool helps floor managers monitor production stages, manage consumption calculations, and track process loss in real-time.

## 🚀 Features

* **Live Production Tracking:** Real-time visibility into garment production stages.
* **Unit-Specific Metrics:** Automatically toggles between **KG** (for Yarn, Knitting, Dyeing, Finishing) and **pcs** (for Cutting, Printing, Sewing, QC, Packaging).
* **Consumption Calculator:** Built-in logic to determine required fabric (KG) based on production pieces and consumption rates.
* **Process Loss Monitoring:** Compare "Planned Loss %" vs "Actual Loss %" for every department.
* **Access Control:** Role-based access (Viewer/Editor) secured by a configurable PIN.
* **Size-wise Order Entry:** Manage orders with granular control over size breakdowns (XS to XXXL).

## 🛠 Tech Stack

* **Frontend:** HTML5, Tailwind CSS, JavaScript (ES6+).
* **Storage/Sync:** Real-time synchronization via MQTT broker.
* **Deployment:** Hosted via GitHub Pages.

## ⚙️ How it Works

1. **Access:** Users start in **Viewer Mode**. Click the **Editor** button and enter the factory-authorized PIN (DM me for reference) to modify production data.
2. **Order Management:** Click **"+ New Order"** to define a new production run, including Buyer details, Style references, and Size-wise quantities.
3. **Data Updates:** Click on any Department Lane to update Received, Output, Alteration, or Rejected quantities. The app automatically calculates WIP and process loss.
4. **Sync:** Use the **"Sync"** button to export your current state as a JSON file for backup.

## 📥 Installation

Since this is a static web application:

1. **Clone the repository:**
   `git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git`
2. **Run:** Open `index.html` in any modern web browser.
3. **Hosting:** Enable **GitHub Pages** in your repository settings (**Settings > Pages**) to make your app live.
