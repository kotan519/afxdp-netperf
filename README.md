# afxdp-netperf

AF_XDPを用いたnetperf相当のUDP RTT計測ツール

## 概要
- XDPでICMP/UDPパケットのみをredirect
- userspace AF_XDPではin-placeでecho replyを生成
- sender側でRTT/jitterを計測（Go 実装）
- kernel stack / OVS / VM は使用しない

