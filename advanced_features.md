# Advanced Features of MonkeyLang

## **1. Networking Tools**
### **1.1 Ping a Host**
```monkeylang
create function ping_host with parameter host
    send ping to host
    if ping successful then
        show "Host is online"
    else
        show "Host is offline"
    end
end

call ping_host with "google.com"
```

### **1.2 Port Scanning**
```monkeylang
create function scan_ports with parameter target_ip
    create port_list as [80, 443, 8080]
    for each port in port_list do
        send connection request to target_ip on port
        if connection successful then
            show "Port " + port + " is open"
        else
            show "Port " + port + " is closed"
        end
    end
end

call scan_ports with "192.168.1.1"
```

## **2. Encryption**
### **2.1 Simple Encryption**
```monkeylang
create function encrypt_data with parameter data, key
    create variable encrypted_data as perform encryption on data using key
    return encrypted_data
end
```

This allows easy **data security** and **safe communication**.
