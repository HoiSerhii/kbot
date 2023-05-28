## kbot
DevOps project from scratch

## Steps in this project

# Step 1. Init go.mod
```
 go mod init github.com/HoiSerhii/kbot
```

# Step 2. Install cobra-cli
```
 go install github.com/spf13/cobra-cli@latest
```

# Step 3. Init default cobra-cli 
```
cobra-cli init
```

# Step 4. Add flags for program
```
cobra-cli add version
cobra-cli add kbot
```

# Step 5. Modify cmd/version.go and add variable 'appVersion'
```
cobra-cli add version
cobra-cli add kbot
```

# Step 6. Build with update variable 'appVersion'
```
 go build -ldflags="-X 'github.com/HoiSerhii/kbot/cmd.appVersion=v1.0.0'"
```

Do not forget 
```
gofmt -s -w ./
```


For save token env (safe)
```
read -s TELE_TOKEN
```

Bot address: http://t.me/devops_test_kbot