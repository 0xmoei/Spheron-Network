## 1. Download script
1. Head over to fizz.spheron.network.
2. Click Connect Wallet to link your wallet.
3. Navigate to View My Fizz to open your Fizz dashboard.
3. At the top, find the Setup tab and open the Installation page.
4. Download the latest script by clicking on the `Download Now` button.
5. `fizzup-v1.0.1.sh` script file will be downloaded to your PC. Send it to your VPS root directory using Mobaxterm or Termius Clients

## 2. Run Script
```
chmod +x /root/fizzup-v1.0.1.sh
```
```
./fizzup-v1.0.1.sh
```

![Screenshot_432](https://github.com/user-attachments/assets/a6568565-9532-4268-a322-ba6d8fcafd3c)

* After a while you get the logs like picture above: `Health check ack received.`
* To exit: `Ctrl+C`


## 3. Check Node health
After running the script, head back to your dashboard and verify:
* Fizz Node Version: It should display v1.1.0
* Fizz Script Version: It should display **v1.0.1**

![Screenshot_430](https://github.com/user-attachments/assets/2c283e24-3645-4449-aadc-256cb08b590d)
