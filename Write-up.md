# RSA1
## Đề bài

## Cách giải

# RSA2
## Đề bài
[small_primes.txt](https://github.com/LuluL0g1n/RSA-CTFd/files/8230912/small_primes.txt)

## Cách giải
>Đưa n lên alpetron
>Dễ dàng tìm được phi = 9535271629301589525422576327693640998475630016999686925425224437013127985147802319031537598149797844942164796406426778044571228816186195955328110080000
```python
from Crypto.Util.number import long_to_bytes
n = 9535271629301589543980737788527614014746809465076973703910968482522722398246280610827753553656401385478044310802319122874965273190562705759366029705507
e = 65537
c = 4552577387909336101290973882061311505705840831095295560114130894123462456438533356021283525714896620886904381766963261172543338282153176336375423711746
phi= 9535271629301589525422576327693640998475630016999686925425224437013127985147802319031537598149797844942164796406426778044571228816186195955328110080000
d = pow(e,-1,phi)
p = pow(c,d,n)
print(long_to_bytes(p))
```
>Flag: KCSC{sm4ll_pr1m3s_RSA}
# RSA3
## Đề bài
```py
from Crypto.Util.number import getPrime, long_to_bytes, bytes_to_long

p = getPrime(1024)
q = getPrime(1024)
n = p*q
e1 = 65537
e2 = 75149

flag = b"KCSC{??????????????????????????????}"
flag = bytes_to_long(flag)


print("n =", n)
print("e1 =", e1)
print("e2 =", e2)
print("c1 =", pow(flag, e1, n))
print("c2 =", pow(flag, e2, n))
```
## Cách giải

# RSA4
## Đề bài

## Cách giải

# RSA5
## Đề bài

## Cách giải

# RSA6
## Đề bài

## Cách giải

# RSA7
## Đề bài

## Cách giải
