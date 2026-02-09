# GTM Stack Data Sync Mesh

A high-fidelity, dark-mode dashboard designed for monitoring complex Revenue Operations (RevOps) data pipelines. This application visualizes real-time sync operations between major GTM systems (Salesforce, HubSpot, Stripe) and internal event buses.

## 🚀 Features

*   **Real-time Metrics:** Live updates for Ingest rates, Data cleanliness, Routing throughput, and Signal processing.
*   **Visual Mesh Map:** An interactive, animated graph visualization showing data flow between satellite nodes and the central event bus.
*   **Pipeline Monitoring:** Detailed table view of active sync nodes with status indicators and latency tracking.
*   **Interactive Elements:** Hover tooltips on mesh nodes provide instant deep-dive statistics.
*   **Glassmorphism UI:** Modern, dark-themed aesthetic with backdrop blurs and subtle gradients.
*   **Responsive Animations:** Smooth transitions and data flow simulations using Framer Motion.

## 🛠️ Tech Stack

*   **Framework:** React 19
*   **Styling:** Tailwind CSS
*   **Animations:** Framer Motion
*   **Icons:** Lucide React
*   **Font:** Inter & JetBrains Mono

## 📂 Project Structure

The core logic resides in a single, self-contained component for easy portability:

*   `components/RevOpsDashboard.tsx`: Main dashboard component containing state logic, data simulation, and UI rendering.
*   `App.tsx`: Root wrapper centering the dashboard.
*   `index.html`: Entry point with global styles and font definitions.

## 🎨 Design System

*   **Theme:** Dark Mode (`bg-[#0f111a]`)
*   **Primary Color:** Indigo (`#5a5cf2`)
*   **Status Colors:**
    *   Online/Healthy: Emerald
    *   Processing/Info: Sky Blue
    *   Warning/Active: Fuchsia
*   **Typography:** 'Inter' for UI text, 'JetBrains Mono' for numbers and code.

## 📦 Usage

This component is designed to be dropped into an existing React application.

1.  Ensure you have Tailwind CSS configured.
2.  Install dependencies:
    ```bash
    npm install framer-motion lucide-react
    ```
3.  Import and use the component:
    ```tsx
    import RevOpsDashboard from './components/RevOpsDashboard';

    function App() {
      return <RevOpsDashboard />;
    }
    ```