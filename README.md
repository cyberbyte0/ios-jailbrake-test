# iOS Jailbreak / Sideload Detector (Web-based)

## Description
This is a lightweight, web-based tool (implemented in `index.html`) designed to detect signs of jailbreaking or sideloading on iOS devices. It runs directly in Safari and uses a combination of non-intrusive browser checks and URL scheme probes to identify potential modifications without requiring app installation.

## Key Features and Advantages
- **Multi-Layer Detection**: Performs soft (informational) checks on browser APIs (e.g., User-Agent, storage, automation headers) and intrusive URL scheme tests for known tools like Cydia, Sileo, Dopamine, Scarlet, and Esign.
- **Enhanced UI/UX**: Features a modern, responsive design with full **Dark Mode** support.
- **Data Portability**: Includes tools to **Export Logs** (.txt) and **Copy Summary** for easy sharing and analysis.
- **User-Friendly Interface**: Includes a progress bar, real-time logs, and a risk score for quick interpretation.
- **No Dependencies**: Pure HTML, CSS, and JavaScript—runs entirely in the browser with no server-side components.
- **Privacy-Focused**: Non-intrusive by default; intrusive checks are optional and clearly indicated.
- **Advantages**: Quick to deploy, no native code needed, educational for understanding iOS security indicators, and effective for basic detection in controlled environments.

## Limitations or Drawbacks
- **False Negatives**: Stealth jailbreaks (e.g., Dopamine with hiding enabled) may evade detection by masking schemes or traces.
- **Browser Restrictions**: Limited to what Safari exposes; cannot access file systems, full app lists, or native APIs, leading to incomplete coverage.
- **iOS-Only**: Optimized for Safari on iPhone/iPad; may not function correctly on other platforms or browsers.
- **Intrusive Nature**: URL scheme checks may trigger app openings or dialogs, which could be disruptive.
- **No Guarantees**: Absence of detections does not confirm a clean device; advanced evasion techniques can bypass it.

## Basic Usage Instructions
1. Open `index.html` in Safari on an iPhone or iPad.
2. Click **Start Full Scan** to run both soft and intrusive checks, or **Quick Scan** for non-intrusive tests.
3. Monitor the progress bar, test tiles, and log area for results.
4. Review the risk score (percentage) and use the **Export Logs** or **Copy Summary** utilities if needed.
5. For best results, test on a physical device; other platforms will show a warning popup and may yield inaccurate outcomes.

## Dependencies or Requirements
- **Browser**: Safari on iOS (iPhone/iPad recommended; tested on iOS 15+).
- **No External Dependencies**: Self-contained HTML file—no libraries, frameworks, or installations required.
- **Optional**: For development, a text editor to modify the script; ensure JavaScript is enabled in the browser.