### Features
* Register new account
* Change license key to use existing Warp+ subscription
* Generate WireGuard profile
* Print trace information to debug Warp/Warp+ status

### Install for Ubuntu
```
bash -c "$(wget -qO- https://raw.githubusercontent.com/OPPAINONYMOUS/wgcf/main/install-wgcf.sh)"
```
### Register new account
Run the following command in a terminal:
```
wgcf register
```
The new account will be saved under wgcf-account.toml
### Generate WireGuard profile
Run the following command in a terminal:
```
wgcf generate
```
The WireGuard profile will be saved under wgcf-profile.conf.
### Change license key
using an environment variable:
```
WGCF_LICENSE_KEY="123412341234" wgcf update
```
### Check device status
Run the following command in a terminal:
```
wgcf status
```
### Verify Warp/Warp+ works
```
wgcf trace
```
If you look at the last line, it should say warp=on or warp=plus, depending on whether you have Warp or Warp+ respectively.
