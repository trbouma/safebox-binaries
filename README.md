# safebox-binaries
Safebox binary files

## Download Mac binary
```
curl -O https://raw.githubusercontent.com/trbouma/safebox-binaries/main/mac-os/safebox
chmod +x ./safebox
./safebox
```

## Download Ubuntu binary
```
curl -O https://raw.githubusercontent.com/trbouma/safebox-binaries/main/ubuntu/safebox
chmod +x ./safebox
./safebox
```

If all goes well, you should see the following:
```
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 24.7M  100 24.7M    0     0  25.9M      0 --:--:-- --:--:-- --:--:-- 25.9M
Usage: safebox [OPTIONS] COMMAND [ARGS]...

Options:
  --help  Show this message and exit.

Commands:
  accept     Accept cashu token
  balance    show balance
  check      Check for payment
  delete     Delete proofs
  deposit    deposit funds into wallet via lightning invoice
  get        get a private wallet record
  info       display info
  init       initialize a new safebox
  issue      Issue token amount
  pay        Payout funds to lightning address
  post       Do a post
  profile    display nostr profile
  proofs     list proofs
  put        help for put
  receive    Receive cashu token
  replicate  replicate safebox data to other relays
  send       Send amount to npub
  set        set local config options
  swap       swap proofs for new proofs
  testpay    Test pay amount
  withdraw   withdraw funds from wallet via lightning invoice
  zap        Zap amount to event or to recipient

```

To see your local default configuration settings, run
```
./safebox set
```

Getting your first funds, say for example depositing 21 sats, run
```
./safebox deposit 21
```

Scan the QR code or copy/paste the lightning invoice. Once you have paid, run

```
./safebox check invoice
./safebox balance
```
If all goes well, you should see that you have 21 sats

more to come...