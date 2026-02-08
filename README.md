# userspace-afxdp-netperf

userspace AF_XDP を用いた netperf 相当の UDP RTT 計測ツール。

## 概要
- XDP で ICMP / UDP パケットのみを redirect
- userspace AF_XDP では in-place で echo reply を生成
- sender 側で RTT / jitter を計測（Go 実装）
- kernel stack / OVS / VM は使用しない

