# Azure VM and Gesture Control Integration

This project integrates Azure Virtual Machine creation with hand gesture control using computer vision. The first component utilizes Azure CLI credentials to establish a connection and create a virtual network interface (NIC) along with a Windows VM, configured with a specific hardware profile and a pre-defined Windows Server image, including secure login credentials.

The second component employs `cvzone`'s HandTrackingModule to recognize hand gestures from an image. Depending on the gesture detected, the application opens Notepad when all fingers are raised, opens Chrome for specific fingers, or outputs "idk" for unrecognized gestures.
