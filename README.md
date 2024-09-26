# Azure VM and Gesture Control Integration
It combines of Azure Virtual Machine creation and a simple hand gesture-based control using computer vision.
The first part connects to Azure using the Azure CLI credentials and creates a virtual network interface (NIC) and a Windows VM. The VM uses a specific hardware profile and a pre-configured Windows Server image, with a username and password set for login.

The second part uses cvzone's HandTrackingModule to detect hand gestures from a photo. Based on the detected finger positions, it opens Notepad if all fingers are up, Chrome if only the index and middle fingers are up, or prints "idk" for other gestures.
