#!/bin/bash

# Xóa tất cả các luật hiện có trong chain INPUT
iptables -F INPUT

# Cho phép các kết nối đến các cổng 80 và 443 từ các địa chỉ IP trong danh sách
iptables -A INPUT -p tcp --dport 80 -s 103.21.244.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 103.21.244.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 103.22.200.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 103.22.200.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 103.31.4.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 103.31.4.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 104.16.0.0/13 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 104.16.0.0/13 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 104.24.0.0/14 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 104.24.0.0/14 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 108.162.192.0/18 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 108.162.192.0/18 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 131.0.72.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 131.0.72.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 141.101.64.0/18 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 141.101.64.0/18 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 162.158.0.0/15 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 162.158.0.0/15 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 172.64.0.0/13 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 172.64.0.0/13 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 173.245.48.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 173.245.48.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 188.114.96.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 188.114.96.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 190.93.240.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 190.93.240.0/20 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 197.234.240.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 197.234.240.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -s 198.41.128.0/17 -j ACCEPT
iptables -A INPUT -p tcp --dport 443 -s 198.41.128.0/17 -j ACCEPT

# Block tất cả các kết nối đến các cổng 80 và 443
iptables -A INPUT -p tcp --dport 80 -j DROP
iptables -A INPUT -p tcp --dport 443 -j DROP

# Lưu cấu hình iptables
iptables-save > /etc/sysconfig/iptables
