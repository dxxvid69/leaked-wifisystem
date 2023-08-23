
package main

import (
    "fmt"
    "time"
)

type WiFiModule struct {
    connected bool
}

func (w *WiFiModule) Connect(ssid, password string) bool {
    fmt.Printf("Connecting to %s...\n", ssid)
    // Simulate connection process
    time.Sleep(time.Second)
    w.connected = true
    return true
}

func (w *WiFiModule) Disconnect() {
    w.connected = false
    fmt.Println("Disconnected")
}

func (w *WiFiModule) IsConnected() bool {
    return w.connected
}

func main() {
    wifi := WiFiModule{}
    
    ssid := "MyWiFiNetwork"
    password := "MyPassword"

    if wifi.Connect(ssid, password) {
        fmt.Println("Connected to WiFi")
    } else {
        fmt.Println("Connection failed")
    }

    if wifi.IsConnected() {
        fmt.Println("Sending data over WiFi...")
        // Simulate data transmission
        time.Sleep(2 * time.Second)
        fmt.Println("Data sent successfully")
    }
    
    wifi.Disconnect()
}
